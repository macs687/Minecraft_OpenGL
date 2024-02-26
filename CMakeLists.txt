cmake_minimum_required(VERSION 3.27.9 FATAL_ERROR)

set(PROJECT_NAME Minecraft_Vulkan)
project(${PROJECT_NAME})

set(CMAKE_CXX_STANDARD 20)

add_executable(${PROJECT_NAME}
    src/Voxel_Engine.cpp

)

find_package(Vulkan REQUIRED)
target_link_libraries(${PROJECT_NAME} Vulkan::Vulkan)
