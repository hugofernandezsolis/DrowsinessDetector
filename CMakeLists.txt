# CMake configurations
cmake_minimum_required(VERSION 3.10)

# Project configurations
set(PROJECT DrowsinessDetector)
project(${PROJECT})
find_package(OpenCV REQUIRED)
include_directories(${OpenCV_INCLUDE_DIRS} ./lib ./src)

# Compiler output
add_executable(${PROJECT} ./src/main.cpp)
target_link_libraries(${PROJECT} ${OpenCV_LIBS})