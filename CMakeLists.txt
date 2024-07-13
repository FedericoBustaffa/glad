
set(CMAKE_C_STANDARD 11)


file(GLOB_RECURSE HEADERS "include/**.h")
file(GLOB_RECURSE SOURCES "src/**.c")

add_library(glad STATIC ${HEADERS} ${SOURCES})

target_include_directories(glad PUBLIC "include/")
