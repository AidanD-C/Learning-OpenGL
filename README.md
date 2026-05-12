# Learning OpenGL
This is a repo where I am learning about OpenGL through [learnopengl.com](https://learnopengl.com). The goal is to use OpenGL to create my own plotting program which will be useful in creating physics animations.

## Dependencies

This project requires GLFW. Download and compile GLFW from [glfw.org/download.html](https://www.glfw.org/download.html), then update the paths in `CMakeLists.txt` to point to your compiled library and headers.

In `CMakeLists.txt`:
```cmake
include_directories(
    "path to your GLFW include directory"
    "include"
)

link_directories("path to your GLFW lib directory")
```