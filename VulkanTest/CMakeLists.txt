cmake_minimum_required(VERSION 3.16)

project(
    VulkanTest
    LANGUAGES CXX
)

set (CMAKE_CXX_STANDARD 17)

find_package(Vulkan REQUIRED)
find_package(glfw3 REQUIRED)

add_executable(vulkan_test)

target_sources(vulkan_test PRIVATE main.cpp)

target_link_libraries(vulkan_test PRIVATE Vulkan::Vulkan glfw)