cmake_minimum_required(VERSION 3.10)
project(BezierCurve)
set(OpenCV_DIR /usr/local/Cellar/opencv@2/2.4.13.7_12.reinstall/share/OpenCV)
find_package(OpenCV REQUIRED)

set(CMAKE_CXX_STANDARD 14)

add_executable(BezierCurve main.cpp)

target_link_libraries(BezierCurve ${OpenCV_LIBRARIES})
