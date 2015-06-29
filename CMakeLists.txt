cmake_minimum_required(VERSION 2.8.0)
project(Tutorial)

include(cmake/macro_function.cmake)
my_macro(TARGETS foo bar DESTINATION bin OPTIONAL blub)
