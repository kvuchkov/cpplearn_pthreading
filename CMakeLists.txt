cmake_minimum_required (VERSION 2.6)
project (pthreading)
find_package (Threads)
include_directories(include)
file(GLOB SOURCES "src/*.cpp")
add_executable(pthreading ${SOURCES})
target_link_libraries (pthreading ${CMAKE_THREAD_LIBS_INIT})