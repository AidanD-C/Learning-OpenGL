cmake_minimum_required(VERSION 3.10)
project(LearnOpenGL)

set(CMAKE_CXX_STANDARD 17)

include_directories(
    "C:/Users/dcaid/Git repos/cpp_libs/opengl_libs/include"
    "include"
)

link_directories("C:/Users/dcaid/Git repos/cpp_libs/opengl_libs/lib")

file(GLOB SOURCES "src/*.cpp" "src/*.c")
add_executable(program ${SOURCES})

target_link_libraries(program glfw3 opengl32)