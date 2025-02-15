cmake_minimum_required(VERSION 3.28)
project(helloworld)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "${PROJECT_SOURCE_DIR}/bin")

message("ROOT CMake Script")
include_directories(lib/include)
add_subdirectory(lib)
add_subdirectory(src)