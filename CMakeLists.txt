cmake_minimum_required(VERSION 3.16)
project(opengl_triangle LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(OpenGL REQUIRED)
find_package(glfw3 REQUIRED)

add_executable(opengl_triangle main.cpp)

target_link_libraries(opengl_triangle PRIVATE glfw OpenGL::GL)
