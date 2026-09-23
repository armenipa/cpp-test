cmake_minimum_required(VERSION 3.20)

project(hello_world
    VERSION 1.0.0
    DESCRIPTION "A modern C++ Hello World application"
    LANGUAGES CXX
)

add_executable(hello_world src/main.cpp)

target_compile_features(hello_world PRIVATE cxx_std_23)

if(MSVC)
    target_compile_options(hello_world PRIVATE /W4 /permissive-)
else()
    target_compile_options(hello_world PRIVATE -Wall -Wextra -Wpedantic)
endif()
