### create build folder

```bash
cmake -B build
```

### create executable

```bash
cmake --build build 
```

or

```bash
cd build
make
```

### Removing build folder
```
cmake -E remove_directory build
```
### Making executable manually

```bash
g++ -o helloworld main.cpp
```

### Windows (MinGW)

```bash
    cmake -B build -G "MinGW Makefiles"
```

```bash
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
5. **include_directories**: Searches for header files inside specified folder
6. **add_subdirectory**: Runs CMake scripts in specified folder
7. **add_library**: Creates library using linked files
8. **target_link_libraries**: Links library to another target. Terminiology: Target=executable or library

### Configure VSCODE

- Press F1 and type CMake: Configure
- Select the Kit/Compiler: If you have multiple compilers or environments set up, you'll be prompted to select one when configuring your CMake project
