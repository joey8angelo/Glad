cmake_minimum_required(VERSION 3.20)
project(glad VERSION 1.0 LANGUAGES CXX)

add_library(glad)

set_target_properties(glad PROPERTIES
    C_STANDARD 20
    C_STANDARD_REQUIRED ON
    C_EXTENSIONS OFF
)

target_sources(glad PRIVATE "src/glad.c")

target_include_directories(glad PUBLIC "include")

