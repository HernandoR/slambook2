cmake_minimum_required(VERSION 2.8)
project(chapter3)

set(CMAKE_CXX_FLAGS "-std=c++14")
include_directories("/usr/local/includes/eigen3")
# 加入各子工程
add_subdirectory(useEigen)
add_subdirectory(useGeometry)
add_subdirectory(visualizeGeometry)
add_subdirectory(examples)
