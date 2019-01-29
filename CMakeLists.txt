# Updated for static linkage by madmaxoft
cmake_minimum_required(VERSION 2.8)
project(lzlib C)

add_library(lzlib STATIC
	lzlib.c
)

target_link_libraries(lzlib lua zlibstatic)
