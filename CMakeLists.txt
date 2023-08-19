cmake_minimum_required(VERSION 3.10)

set(CMAKE_MODULE_PATH "${CMAKE_SOURCE_DIR}/cmake_modules" ${CMAKE_MODULE_PATH})

project(Game)

find_package(SFML COMPONENTS system window graphics CONFIG REQUIRED)

add_executable(Game main.cpp)
target_link_libraries(Game PRIVATE sfml-system sfml-network sfml-graphics sfml-window)
