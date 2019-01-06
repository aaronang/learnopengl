cmake_minimum_required(VERSION 3.12)

project(triangles)

add_executable(triangles src/main.cpp)

find_package(glfw3 REQUIRED)

target_link_libraries(triangles
        glfw
        glad
        )