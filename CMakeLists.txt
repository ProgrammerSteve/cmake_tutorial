cmake_minimum_required(VERSION 3.28)
project(helloworld)

message("ROOT CMake Script")
add_subdirectory(lib)
add_subdirectory(src)

add_executable(helloworld main.cpp add.cpp)