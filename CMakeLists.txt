cmake_minimum_required(VERSION 2.8)
project(AnyOption)

set(AnyOption_SRCS anyoption.cpp)
set(AnyOption_HDRS anyoption.h)

include_directories(.)

add_library(AnyOption SHARED ${AnyOption_SRCS} ${AnyOption_HDRS})

add_executable(demo demo.cpp ${AnyOption_SRCS})

