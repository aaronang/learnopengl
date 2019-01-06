cmake_minimum_required(VERSION 3.12)

project(playground)

add_executable(playground src/main.cpp)

find_package(glfw3 REQUIRED)

target_link_libraries(playground
        glfw
        glad
        )