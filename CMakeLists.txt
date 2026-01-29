cmake_minimum_required(VERSION 4.2.1)
project(cpp-project-tmpl VERSION 0.0.1 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 26)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
set(CMAKE_CXX_EXTENSIONS OFF)

include(FetchContent)

find_package(Catch2 3 REQUIRED)

include(cmake/utils.cmake)

add_subdirectory(src)
add_subdirectory(apps)
add_subdirectory(tests)
