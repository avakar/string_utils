cmake_minimum_required(VERSION 3.0)
project(string_utils)

include(deps.cmake)

add_library(string_utils src/string_utils.cpp)
target_include_directories(string_utils PUBLIC include)
target_link_libraries(string_utils string_view)
