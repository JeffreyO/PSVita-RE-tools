cmake_minimum_required(VERSION 3.13)
project(elf_injector)
# set(CMAKE_C_STANDARD)
# set(CMAKE_CXX_STANDARD)

find_library(LIB_Z z REQUIRED)

set(SOURCE_FILES
main.c
sha256.c
)

add_executable(${PROJECT_NAME} ${SOURCE_FILES})
target_link_libraries(${PROJECT_NAME} ${LIB_Z})
