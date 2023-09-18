#设定最低运行的CMake版本
cmake_minimum_required(VERSION 3.10)
#项目生成的exe文件名字
project(demo)
#找出所有源文件c的文件夹
file(GLOB SRC ${CMAKE_CURRENT_SOURCE_DIR}/src/*.cpp)
#包含所有的头文件
include_directories(${PROJECT_SOURCE_DIR}/include)
#添加头文件的源地址
add_executable(demo ${SRC})
