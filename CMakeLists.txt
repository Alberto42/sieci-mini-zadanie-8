cmake_minimum_required(VERSION 3.8)
project(SIK_8)

set(CMAKE_C_STANDARD 99)
set (CMAKE_C_FLAGS "-Wall")

add_executable(server server.c err.h err.c)
add_executable(client client.c err.c err.h)