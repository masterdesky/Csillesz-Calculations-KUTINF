#Specify the minimum version for CMake

cmake_minimum_required(VERSION 2.8.12)

# Project's name

project(csill)
# Set the output folder where your program will be created
set(CMAKE_BINARY_DIR ${CMAKE_SOURCE_DIR}/build)
set(EXECUTABLE_OUTPUT_PATH ${CMAKE_BINARY_DIR})
set(LIBRARY_OUTPUT_PATH ${CMAKE_BINARY_DIR})

# The following folder will be included
include_directories("${PROJECT_SOURCE_DIR}")

# Executable
add_executable(csill ${PROJECT_SOURCE_DIR}/csill.cpp)
