cmake_minimum_required(VERSION 3.12)

project(glad)

add_library(glad src/glad.c)

target_include_directories(glad
        PUBLIC
        $<INSTALL_INTERFACE:include>
        $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include>
        PRIVATE
        ${CMAKE_CURRENT_SOURCE_DIR}/src
        )

target_link_libraries(glad
        PRIVATE
        ${CMAKE_DL_LIBS}
        )