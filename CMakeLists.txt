cmake_minimum_required(VERSION 3.14)

project(optim-sample)

set(CMAKE_CXX_STANDARD 11)

add_executable(sample main.cpp)

find_package(Armadillo CONFIG REQUIRED)
target_link_libraries(sample PRIVATE ${ARMADILLO_LIBRARIES})