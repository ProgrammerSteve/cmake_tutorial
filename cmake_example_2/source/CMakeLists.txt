#Link executable to source file
add_executable(calculator main.cpp)

#Link "math" library to executable
target_link_libraries(calculator math)