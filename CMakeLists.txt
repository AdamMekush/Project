cmake_minimum_required(VERSION 3.10)
project(Project)

set(BUILD_CURL_EXE OFF CACHE INTERNAL "Set to ON to build curl executable.")

set(BUILD_SHARED_LIBS ON)

set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY "${PROJECT_BINARY_DIR}")
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY "${CMAKE_SOURCE_DIR}/bin")
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "${CMAKE_SOURCE_DIR}/bin")

add_subdirectory("src")
add_subdirectory("libs/curl")
add_subdirectory("libs/json")


