cmake_minimum_required(VERSION 3.31)
project(untitledlog)

set(CMAKE_CXX_STANDARD 23)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

# collect all the files
file(GLOB_RECURSE SOURCES "src/*.cpp")

add_library(untitledlog SHARED ${SOURCES})

target_include_directories(untitledlog PUBLIC include)