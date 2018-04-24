cmake_minimum_required(VERSION 3.8)
project(SIK_8)

set(CMAKE_C_STANDARD 99)

set(SOURCE_FILES main.c)
set (CMAKE_C_FLAGS "-levent")
SET( CMAKE_EXE_LINKER_FLAGS  "-levent")
    add_executable(SIK_8 ${SOURCE_FILES})

add_executable(server server.c err.h err.c)
add_executable(client client.c err.c err.h)