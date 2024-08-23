cmake_minimum_required(VERSION 3.27)
project(shazam)

set(CMAKE_CXX_STANDARD 11)

add_executable(shazam_demo main.c)
target_link_libraries(shazam_demo -lm)
