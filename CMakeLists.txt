cmake_minimum_required(VERSION 2.8 FATAL_ERROR)

set(PROJECT_NAME cpp_app_skeleton)

project(${PROJECT_NAME})

set(CMAKE_CXX_FLAGS "-g -Wall")

set(SOURCE_FILES
	src/main.cc
)

add_executable(${PROJECT_NAME} ${SOURCE_FILES})

add_subdirectory(libs/cpp_lib_skeleton)

target_link_libraries(${PROJECT_NAME} cpp_lib_skeleton)