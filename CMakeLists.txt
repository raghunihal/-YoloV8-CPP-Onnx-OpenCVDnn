cmake_minimum_required(VERSION 3.0.0)
set(CMAKE_BUILD_TYPE "")

project(YoloV8 VERSION 0.1.0)

find_package(OpenCV REQUIRED)

add_executable(YoloV8 YoloV8.cpp)

include_directories(${OpenCV_INCLUDE_DIRS})
target_link_libraries(main ${OpenCV_LIBS} ${CMAKE_THREAD_LIBS_INIT})
