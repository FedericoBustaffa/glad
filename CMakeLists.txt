cmake_minimum_required(VERSION 3.20)

project(glad)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

file(GLOB_RECURSE HEADERS "include/**.h")
file(GLOB_RECURSE SOURCES "src/**.c")

add_library(glad STATIC ${HEADERS} ${SOURCES})

target_include_directories(glad PUBLIC "include/")
