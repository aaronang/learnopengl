cmake_minimum_required(VERSION 3.12)

project(learnopengl)

set(CMAKE_MODULE_PATH "${CMAKE_CURRENT_SOURCE_DIR}/cmake" ${CMAKE_MODULE_PATH})

add_subdirectory(libraries)
add_subdirectory(applications)