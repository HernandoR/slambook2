cmake_minimum_required(VERSION 3.4)
project(slambook)

set(CMAKE_CXX_FLAGS "-std=c++14")
# include_directories("/usr/local/includes/eigen3")
# 加入各子工程
add_subdirectory(ch2)
add_subdirectory(ch3)
add_subdirectory(ch4)
add_subdirectory(ch5)
add_subdirectory(ch6)
add_subdirectory(ch7)
add_subdirectory(ch8)
add_subdirectory(ch9)
add_subdirectory(ch10)
add_subdirectory(ch11)
add_subdirectory(ch12)
add_subdirectory(ch13)

