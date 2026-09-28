cmake_minimum_required(VERSION 3.20)

project(NetLock
    VERSION 0.1.0
    LANGUAGES CXX
)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

add_executable(netlock_client
    client/src/main.cpp
)

target_include_directories(netlock_client PRIVATE
    client/include
    shared/include
)