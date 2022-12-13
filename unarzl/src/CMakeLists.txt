cmake_minimum_required(VERSION 3.13)
project(unarzl)
# set(CMAKE_C_STANDARD)
# set(CMAKE_CXX_STANDARD)

# find_library(LIB_* * REQUIRED)

set(SOURCE_FILES
main.c
unarzl.c
)

add_executable(${PROJECT_NAME} ${SOURCE_FILES})
# target_link_libraries(${PROJECT_NAME} ${LIB_*})
