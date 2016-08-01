cmake_minimum_required(VERSION 2.8)
project(IQRF_LINUX)

set(MACHINE RPI)

if(MACHINE)
	add_definitions(-D${MACHINE})
endif(MACHINE)

add_subdirectory(src)
add_subdirectory(examples)

set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -std=c11 -g")
