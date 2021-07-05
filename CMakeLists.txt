cmake_minimum_required(VERSION 3.17)
project(s_lab3)

set(CMAKE_CXX_STANDARD 14)

add_subdirectory(gtest/googletest)
add_executable(s_lab3 main.cpp Complex.h Heap.h BinaryTree.h func.h func.cpp menu.h menu.cpp test.cpp)
include_directories(googletest/googletest/include)
target_link_libraries(s_lab3 gtest gtest_main)