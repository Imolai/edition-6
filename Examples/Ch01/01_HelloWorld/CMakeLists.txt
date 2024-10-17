cmake_minimum_required(VERSION 3.22)
project(IndependentBinaries CXX)

# Set the C++ standard to C++23
set(CMAKE_CXX_STANDARD 23)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# Explicitly set clang++ as the compiler
set(CMAKE_CXX_COMPILER clang++)
# set(CMAKE_CXX_COMPILER g++)

# Options to build specific executables
option(BUILD_HELLO "Build hello executable" ON)
option(BUILD_PRINTING "Build printing executable" OFF)
option(BUILD_STREAMS "Build streams executable" OFF)
option(BUILD_INPUT "Build input executable" OFF)

# Add executable targets based on user choice
if(BUILD_HELLO)
    add_executable(hello 01_helloworld.cpp)
endif()

if(BUILD_PRINTING)
    add_executable(printing 02_printing.cpp)
endif()

if(BUILD_STREAMS)
    add_executable(streams 03_streams.cpp)
endif()

if(BUILD_INPUT)
    add_executable(input 04_input.cpp)
endif()

# Build:
# cmake .
# make
