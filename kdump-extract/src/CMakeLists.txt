cmake_minimum_required(VERSION 3.13)
project(kdump-extract)
# set(CMAKE_C_STANDARD)
# set(CMAKE_CXX_STANDARD)

set(SOURCE_FILES main.c)

add_executable(${PROJECT_NAME} ${SOURCE_FILES})
target_link_libraries(${PROJECT_NAME})
