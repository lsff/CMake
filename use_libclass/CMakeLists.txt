cmake_minimum_required(VERSION 2.8.0)
project(use_libclass)

add_definitions(-DUNICODE -D_UNICODE)

file(GLOB use_libclass_SOURCES src/*.cpp)

include_directories(../lib_class/src)

add_executable(use_libclass ${use_libclass_SOURCES})

target_link_libraries(use_libclass "D:\\coding\\lib_class\\debug\\Debug\\lib_class.lib") 
