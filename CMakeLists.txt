cmake_minimum_required(VERSION 2.8) 
project(tutorial_prj)

add_subdirectory(poo)
add_subdirectory(foo)

set(source_file main.cpp)
add_executable(tutorial ${source_file})


target_link_libraries(tutorial poo) 
target_link_libraries(tutorial foo) 
