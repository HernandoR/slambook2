cmake_minimum_required(VERSION 3.0)
project(useSophus)

find_package( FMT REQUIRED )
include_directories(${FMT_INCLUDE_DIRS})

# 为使用 sophus，需要使用find_package命令找到它
find_package(Sophus REQUIRED)
include_directories(${Sophus_INCLUDE_DIRS})
# Eigen
include_directories("/usr/include/eigen3")
add_executable(useSophus useSophus.cpp)
target_link_libraries(useSophus ${Sophus_LIBRARIES} ${FMT_LIBRARIES} fmt)

add_subdirectory(example)
