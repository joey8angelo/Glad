cmake_minimum_required(VERSION 3.20)
project(glad LANGUAGES C)

add_library(glad src/glad.c)
target_include_directories(glad PUBLIC include)
target_compile_features(glad PRIVATE c_std_20)
