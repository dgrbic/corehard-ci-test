cmake_minimum_required(VERSION 3.14.0 FATAL_ERROR)
project(hello CXX)
#set(SOURCES
#    src/hello.cpp
#)
file(GLOB SOURCES "src/*.cpp")
message(${SOURCES})
add_executable(${PROJECT_NAME} ${SOURCES})
set_property(TARGET ${PROJECT_NAME} PROPERTY CXX_STANDARD 14)

