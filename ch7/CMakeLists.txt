cmake_minimum_required ( VERSION 2.8 )

project(feature_extraction)

find_package(OpenCV REQUIRED)
include_directories(${OpenCV_INCLUDE_DIRS})

add_executable(feature_extraction feature_extraction.cpp)

target_link_libraries(feature_extraction  ${OpenCV_LIBS})
