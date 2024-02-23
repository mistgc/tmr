cmake_minimum_required(VERSION 3.5)
project(tmr LANGUAGES CXX)

file(GLOB_RECURSE SRC CONFIGURE_DEPENDS
    ${CMAKE_SOURCE_DIR}/src/*.cpp
    ${CMAKE_SOURCE_DIR}/include/*.h
)

add_library(${PROJECT_NAME} STATIC ${SRC})
