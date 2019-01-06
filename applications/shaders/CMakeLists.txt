cmake_minimum_required(VERSION 3.12)

project(shaders)

add_executable(shaders src/main.cpp)

find_package(glfw3 REQUIRED)

target_link_libraries(shaders
        glfw
        glad
        )