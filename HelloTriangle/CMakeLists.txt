cmake_minimum_required(VERSION 3.16)

project(
        HelloTriangle
        LANGUAGES CXX
)

set (CMAKE_CXX_STANDARD 17)

find_package(Vulkan REQUIRED)
find_package(glfw3 REQUIRED)

add_executable(hello_triangle)

target_sources(hello_triangle PRIVATE main.cpp)

target_link_libraries(hello_triangle PRIVATE Vulkan::Vulkan glfw)