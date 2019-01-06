cmake_minimum_required(VERSION 3.12)

project(hellotriangle)

add_executable(hellotriangle src/main.cpp)

find_package(glfw3 REQUIRED)

target_link_libraries(hellotriangle
        glfw
        glad
        )