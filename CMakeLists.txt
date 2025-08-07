cmake_minimum_required(VERSION 3.31)
project(sample-meshcore-through-git-submodule)

set(CMAKE_CXX_STANDARD 20)

set(MESHCORE_BUILD_DEMOS OFF)
add_subdirectory(meshcore)

add_executable(sample main.cpp)
target_link_libraries(sample MeshCore)
