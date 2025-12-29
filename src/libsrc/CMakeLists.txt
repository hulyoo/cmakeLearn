cmake_minimum_required(VERSION 3.0)
project(libsrc)

include_directories(${HEAD_PATH})

aux_source_directory(${CMAKE_CURRENT_SOURCE_DIR} SRC)
message(STATUS "${SRC}")

set(LIBRARY_OUTPUT_PATH ${LIBRARY_PATH})

add_library(libsrc SHARED ${SRC})

