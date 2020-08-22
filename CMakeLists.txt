cmake_minimum_required(VERSION 3.15)

# set the project name
project(indr)

# use C++17 standard
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# compiler flags
set(CMAKE_CXX_FLAGS "-Wall -Wextra -Werror")
set(CMAKE_CXX_FLAGS_DEBUG "-pg")
set(CMAKE_CXX_FLAGS_RELEASE "-O3")

# boost
set(Boost_ADDITIONAL_VERSIONS 1.74)
find_package(Boost REQUIRED COMPONENTS unit_test_framework)

# spdlog
add_subdirectory(include/third_party/spdlog/)

# zlib
add_subdirectory(include/third_party/zlib/)

# set the header includes directory
include_directories(include/)

# enable testing framework
enable_testing()

# add the actual code
add_subdirectory(src)
add_subdirectory(tests)