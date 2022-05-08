cmake_minimum_required(VERSION 3.15)

project(TinySQL)

add_executable(main src/main.c)

include_directories(include)

add_library(InputBuffer STATIC src/InputBuffer.c)

target_link_libraries(main PUBLIC InputBuffer)