cmake_minimum_required(VERSION 3.20)

project(Database-of-Games LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

add_executable(Database-of-Games
    src/main.cpp
    src/games_graph.cpp
    src/sales_tree.cpp
)

target_include_directories(Database-of-Games PRIVATE
    ${CMAKE_CURRENT_SOURCE_DIR}/include
)
