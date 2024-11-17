cmake_minimum_required(VERSION 3.20)

project(proxy   VERSION 1.0
                DESCRIPTION "PROXY librairie for Indoor Weather Station"
                LANGUAGES CXX C)


# ADD .cpp & .h
set(SRC_DIR ${CMAKE_CURRENT_SOURCE_DIR}/src)

set(SRC
    ${SRC_DIR}/proxy.cpp
)


# LINK
add_library(proxy STATIC ${SRC})
target_include_directories(proxy PUBLIC ${SRC_DIR})