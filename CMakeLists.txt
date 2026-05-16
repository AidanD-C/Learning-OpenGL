cmake_minimum_required(VERSION 3.10)
project(LearnOpenGL)

set(CMAKE_CXX_STANDARD 17)

include_directories(
    "C:/Users/dcaid/Git repos/cpp_libs/opengl_libs/include"
    "include"
)

link_directories("C:/Users/dcaid/Git repos/cpp_libs/opengl_libs/lib")

add_executable(main src/main.cpp src/gl.c)
add_executable(exercises src/exercises.cpp src/gl.c)

target_link_libraries(main glfw3 opengl32)
target_link_libraries(exercises glfw3 opengl32)