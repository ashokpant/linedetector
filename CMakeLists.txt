cmake_minimum_required(VERSION 3.16)
project(linedetector)
find_package(OpenCV REQUIRED)
set(CMAKE_CXX_STANDARD 14)

add_executable(linedetection_image src/linedetection_image.cpp src/linedetector.cpp )
target_link_libraries(linedetection_image ${GOOGLE_LIBRARIES} ${OpenCV_LIBS})
add_executable(linedetection_video src/linedetection_video.cpp src/linedetector.cpp )
target_link_libraries(linedetection_video ${GOOGLE_LIBRARIES} ${OpenCV_LIBS})