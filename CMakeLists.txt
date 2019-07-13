cmake_minimum_required(VERSION 3.12)


project(sdb2)


message(STATUS ${CMAKE_SOURCE_DIR}/../uvw/src)
include_directories(
  ${CMAKE_SOURCE_DIR}/../libuv-1.x/include
  ${CMAKE_SOURCE_DIR}/../uvw/src)

add_executable(sdb2 main.cc)
target_link_libraries(sdb2 
