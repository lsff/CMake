cmake_minimum_required(VERSION 2.8.0)
project(lib_class)

add_definitions(-DUNICODE -D_UNICODE)

include_directories(src)

file(GLOB mylib_source src/*.cpp) #message("${mylib_source}")
file(GLOB mylib_header src/*.h) #message("${mylib_header}")

source_group("Source Files"  FILES ${mylib_source})
source_group("Header Files" FILES ${mylib_header})

add_library(lib_class STATIC ${mylib_source} ${mylib_header})
