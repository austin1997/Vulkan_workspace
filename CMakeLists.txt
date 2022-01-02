cmake_minimum_required(VERSION 3.16)

project(
    Vulkan_Workspace
    LANGUAGES CXX
)

set (CMAKE_CXX_STANDARD 17)

find_package(Vulkan REQUIRED)
add_subdirectory(VulkanTest)
