cmake_minimum_required(VERSION 3.20)
project(netmon)

set(CMAKE_CXX_STANDARD 20)

set(SOURCES src/Entry.cpp)

add_executable(netmon ${SOURCES})

target_link_libraries(netmon PRIVATE Walnut thread_master)
target_include_directories(netmon PRIVATE ../../deps/imgui ../../deps/GLFW/include ../../deps/Walnut/Source ../../deps/Walnut/Platform/GUI C:/VulkanSDK/1.3.268.0/Include ../../deps/glm)