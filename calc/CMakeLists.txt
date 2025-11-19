cmake_minimum_required(VERSION 3.10)

project(MyProject)

set(CMAKE_CXX_STANDARD 17)

add_library(oper STATIC
    add.cpp
    mul.cpp
)

add_executable(main
    main.cpp
    add.cpp
    mul.cpp
)
