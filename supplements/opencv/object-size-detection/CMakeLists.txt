cmake_minimum_required(VERSION 2.8)
project( RV )
set(CMAKE_CXX_STANDARD 14)
find_package( OpenCV REQUIRED )
include_directories( ${OpenCV_INCLUDE_DIRS} )
add_executable( RV src/main.cpp )
target_link_libraries( RV ${OpenCV_LIBS} )