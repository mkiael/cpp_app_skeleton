cmake_minimum_required(VERSION 2.8 FATAL_ERROR)

set(PROJECT_NAME cpp_app_skeleton)

project(${PROJECT_NAME})

set(CMAKE_CXX_FLAGS "-g -Wall")

include_directories(include)

set(SOURCE_FILES
	src/main.cc
)

add_executable(cpp_app_skeleton ${SOURCE_FILES})