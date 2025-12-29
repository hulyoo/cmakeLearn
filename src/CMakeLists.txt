CMAKE_MINIMUM_REQUIRED(VERSION 3.0)
project(src)

aux_source_directory(./ SRC_LIST)

include_directories(${HEAD_PATH})
#message(STATUS "${HEAD_PATH}")

set(LIBRARY_OUTPUT_PATH ${LIBRARY_PATH})
# set(EXECUTABLE_OUTPUT_PATH,${PROJECT_SOURCE_DIR}/bin)

# link_directories(${CMAKE_CURRENT_SOURCE_DIR}/lib)

add_library(${LIB_ADD_NAME} STATIC ${SRC_LIST})

add_subdirectory(libsrc)