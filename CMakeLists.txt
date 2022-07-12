# CMake configurations
cmake_minimum_required(VERSION 3.10)

# C++ configurations

# Project configurations
set(PROJECT DrowsinessDetector)
project(${PROJECT})

# Compiler output
add_executable(${PROJECT} main.cpp)