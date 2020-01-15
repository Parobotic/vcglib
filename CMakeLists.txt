cmake_minimum_required(VERSION 3.13.1)

project(vcglib LANGUAGES CXX VERSION 1.0.1)

add_library (vcglib INTERFACE)
add_library (vcglib::vcglib ALIAS vcglib)
target_include_directories (vcglib INTERFACE $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}>)
