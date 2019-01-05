cmake_minimum_required(VERSION 3.12)

project(learnopengl)

list(INSERT CMAKE_MODULE_PATH 0 ${CMAKE_SOURCE_DIR}/cmake)

find_package(glfw3 REQUIRED)

add_executable(learnopengl
        src/glad.c
        src/main.cpp)

target_include_directories(learnopengl
        PUBLIC
        $<INSTALL_INTERFACE:include>
        $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include>
        PRIVATE
        ${CMAKE_CURRENT_SOURCE_DIR}/src
        )

target_link_libraries(learnopengl
        PRIVATE
        glfw
        ${CMAKE_DL_LIBS}
        )