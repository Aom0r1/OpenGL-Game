cmake_minimum_required (VERSION 3.29.0 FATAL_ERROR)

project(BattleCity)

add_executable(BattleCity src/main.cpp)

add_subdirectory(external/glfw)
add_subdirectory(external/glad)

target_link_libraries(BattleCity glfw)
target_link_libraries(BattleCity glad)	