cmake_minimum_required(VERSION 3.3)
project(OpenCVTutorial)
find_package( OpenCV REQUIRED )

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

set(SOURCE_FILES main.cpp)
add_executable(OpenCVTutorial ${SOURCE_FILES})

target_link_libraries( OpenCVTutorial ${OpenCV_LIBS} )