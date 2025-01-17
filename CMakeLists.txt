# CMake version check
cmake_minimum_required(VERSION 3.31)

# Project name
project(das)

# Compiler options
# Enable c++11 standard
set(CMAKE_CXX_STANDARD 11)

# Maximum warning level for g++
set(cxx_warning_options -Wall -Wextra -Wpedantic)
add_compile_options("$<$<CXX_COMPILER_ID:GNU>:${cxx_warning_options}>")

# Treats warnings as errors
set(CMAKE_COMPILE_WARNING_AS_ERROR ON)

# Subdirectories
add_subdirectory(main)
