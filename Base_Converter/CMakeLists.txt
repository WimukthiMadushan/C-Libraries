cmake_minimum_required(VERSION 3.30)
project(Base_Converter)

set(CMAKE_CXX_STANDARD 20)

add_library(Base_Converter STATIC library.cpp)

add_executable(Base_Converter_Main library.cpp)

target_link_libraries(Base_Converter_Main PRIVATE Base_Converter)
