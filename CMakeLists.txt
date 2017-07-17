cmake_minimum_required(VERSION 2.8.3)
project(Eigen_test)
set(CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} ".")
set(CMAKE_MODULE_PATH ${CMAKE_CURRENT_SOURCE_DIR})
find_package(Eigen REQUIRED)
include_directories(
    ${EIGEN_INCLUDE_DIRS}
)
add_executable(Eigen_test Eigen_test.cpp)
