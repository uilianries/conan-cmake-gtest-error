PROJECT(gtest_1)
cmake_minimum_required(VERSION 3.10)

include(${CMAKE_BINARY_DIR}/conanbuildinfo_multi.cmake)
CONAN_BASIC_SETUP(TARGETS)

ADD_EXECUTABLE(gtest_1 main.cpp)
target_link_libraries(gtest_1 CONAN_PKG::gtest)
