cmake_minimum_required(VERSION 3.7)
project(mudserver)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_MODULE_PATH "${CMAKE_SOURCE_DIR}/cmake")

file(GLOB mudserver_src ${CMAKE_SOURCE_DIR}/source/*[c,h]*)
add_executable(mudserver ${mudserver_src})