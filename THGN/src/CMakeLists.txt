cmake_minimum_required(VERSION 3.13)
project(THGNIDS)
# set(CMAKE_C_STANDARD)
# set(CMAKE_CXX_STANDARD)

find_library(LIB_YAML yaml REQUIRED)
find_library(LIB_Z z REQUIRED)

set(SOURCE_FILES
import/vita-import-parse.c
import/vita-import.c
import/yamltree.c
import/yamltreeutil.c
main.cpp
)

add_executable(${PROJECT_NAME} ${SOURCE_FILES})
target_link_libraries(${PROJECT_NAME}
${LIB_YAML}
${LIB_Z}
)
