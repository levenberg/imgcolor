cmake_minimum_required(VERSION 2.8.3)
project(vision)

# add_compile_options(-std=c++11)

find_package(OpenCV REQUIRED)
 add_executable(imgcolor main.cpp)

 target_link_libraries(imgcolor
   ${OpenCV_LIBS}
 )

