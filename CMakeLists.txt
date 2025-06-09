cmake_minimum_required(VERSION 3.29)
project(mathlib LANGUAGES CXX)

file(GLOB CPP_SOURCES src/*.cpp)
file(GLOB IXX_SOURCES src/*.ixx)
set(SRCS ${CPP_SOURCES} ${IXX_SOURCES})
add_module_library(mathlib SRC_LIST ${SRCS})
target_include_directories(mathlib PUBLIC include)
