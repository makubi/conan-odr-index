cmake_minimum_required(VERSION 3.15)

project(odr-test-downstream LANGUAGES C CXX)
set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

find_package(odrcore REQUIRED)

add_executable(odr-test-downstream test_package.cpp)
target_link_libraries(odr-test-downstream PRIVATE odrcore::odrcore)
