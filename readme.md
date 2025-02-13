### create build folder
```
cmake -B build
```
### create executable
```
cmake --build build 
```
or
```
cd build
make
```
### Removing build folder
```
cmake -E remove_directory build
```
### Making executable manually
```
g++ -o helloworld main.cpp
```
### Windows (MinGW)
```
cmake -B build -G "MinGW Makefiles"
```
```
cd build
mingw32-make
```

### 3 commands needed in cmake
- `cmake_minimum_required(VERSION 3.28)`
- `project(helloworld)`
- `add_executable(helloworld main.cpp add.cpp)`



## Fundamental Commands

1. **cmake_minimum_required**: confirms that active cmake is not out of date
2. **project**: determines name of executable file
3. **add_executable**: links targets to executable file
4. **message**: Displays text while cmake is executed
5. **include_directories**
6. **add_subdirectory** Runs CMake scripts in specified folder
7. **add_library**
8. **target_link_libraries**