cmake_minimum_required(VERSION 3.13)
project(PSVita-ELF-builder)
# set(CMAKE_C_STANDARD)
# set(CMAKE_CXX_STANDARD)

find_library(LIB_Z z REQUIRED)

set(SOURCE_FILES
file.c
main.c
)

add_executable(${PROJECT_NAME} ${SOURCE_FILES})
target_link_libraries(${PROJECT_NAME}
${LIB_Z}
)
