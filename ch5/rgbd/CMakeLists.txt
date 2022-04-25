find_package(Sophus REQUIRED)
include_directories(${Sophus_INCLUDE_DIRS})

find_package(Pangolin REQUIRED)
find_package( FMT REQUIRED )
include_directories(${FMT_INCLUDE_DIRS})
set(FMT_LIBRARIES fmt::fmt)

add_executable(joinMap joinMap.cpp)
target_link_libraries(joinMap ${OpenCV_LIBS} ${Pangolin_LIBRARIES} fmt::fmt)