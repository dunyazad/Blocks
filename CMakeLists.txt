cmake_minimum_required(VERSION 3.1)

project(Blocks)

add_subdirectory("External/BlockA")

add_executable(Blocks
src/main.cpp)

target_include_directories(BlockA PUBLIC "External/BlockA/src")

target_link_libraries(Blocks BlockA)
