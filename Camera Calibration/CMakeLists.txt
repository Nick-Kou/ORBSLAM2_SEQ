cmake_minimum_required(VERSION 3.17)
project(CameraCalibration)

set(CMAKE_CXX_STANDARD 14)


find_package( OpenCV REQUIRED )
include_directories( ${OpenCV_INCLUDE_DIRS} )
add_executable(CameraCalibration main.cpp)
target_link_libraries(CameraCalibration ${OpenCV_LIBS} )

