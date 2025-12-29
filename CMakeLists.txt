CMAKE_MINIMUM_REQUIRED(VERSION 3.0)
project(test_cmake)

set(CMAKE_CXX_FLAGS ${CMAKE_CXX_FLAGS} -g)

set(HEAD_PATH ${PROJECT_SOURCE_DIR}/include)
#message(STATUS "${PROJECT_SOURCE_DIR}/include")

set(LIBRARY_PATH ${PROJECT_SOURCE_DIR}/lib)
set(EXE_PATH ${PROJECT_SOURCE_DIR}/bin)

set(LIB_ADD_NAME libadd)
set(LIB_SUB_NAME libsub)
set(LIB_LIB_NAME libsrc)

add_subdirectory(src)
add_subdirectory(example)
