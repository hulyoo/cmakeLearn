cmake_minimum_required(VERSION 3.0)
project(example)


set(EXECUTABLE_OUTPUT_PATH ${EXE_PATH})
#message(STATUS "${EXECUTABLE_OUTPUT_PATH}")
# message(STATUS "${EXE_PATH}")
include_directories(${HEAD_PATH})
aux_source_directory(. SRC_LIST)

link_directories(${LIBRARY_PATH})
link_libraries(${LIB_ADD_NAME})

add_executable(test_add ${SRC_LIST})

target_link_libraries(test_add ${LIB_LIB_NAME})

