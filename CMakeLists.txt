cmake_minimum_required(VERSION 3.25)
project(jni_starter)

set(CMAKE_BUILD_TYPE Release)
set(CMAKE_CXX_STANDARD 17)

find_package(JNI REQUIRED)
include_directories(${JNI_INCLUDE_DIR})

set(SOURCE_FILES src/main.cpp)

add_library(jni_starter SHARED ${SOURCE_FILES})
