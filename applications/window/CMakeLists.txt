cmake_minimum_required(VERSION 3.12)

project(window)

add_executable(window src/main.cpp)

find_package(glfw3 REQUIRED)

target_link_libraries(window
        glfw
        glad
        )