cmake_minimum_required(VERSION 3.15)
project(argv_parsing VERSION 1.0 LANGUAGES C)

set(INCLUDE_DIR "${CMAKE_SOURCE_DIR}/include")
set(SRC_DIR "${CMAKE_SOURCE_DIR}/src")

add_library(argv_parsing ${SRC_DIR}/argv_parsing.c)

target_include_directories(argv_parsing PUBLIC ${INCLUDE_DIR})
