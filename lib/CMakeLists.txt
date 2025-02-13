message("LIB CMake Script")

add_subdirectory(lib)
add_subdirectory(src)

message("abcdefgh")
add_executable(helloworld main.cpp add.cpp)