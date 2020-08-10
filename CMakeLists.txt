cmake_minimum_required(VERSION 3.17)
project(Minecraft)

set(CMAKE_CXX_STANDARD 14)

include_directories(include)

link_directories(lib)

add_executable(Minecraft src/main.cpp src/common/Shader.cpp src/common/Shader.hpp)

target_link_libraries(Minecraft glew32s glfw3 opengl32)