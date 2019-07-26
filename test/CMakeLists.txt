# cmake_minimum_required(VERSION <specify CMake version here>)
# 1.project name，指定项目的名称，一般和项目的文件夹名称对应
project(test C)

# 2.set environment variable，设置环境变量，编译用到的源文件全部都要放到这里，否则编译能够通过
#，但是执行的时候会出现各种问题，比如"symbol lookup error xxxxx , undefined symbol"
set(CMAKE_C_STANDARD 99)

# 3.add executable file，添加要编译的可执行文件
add_executable(test files/DataType/DataType.c)