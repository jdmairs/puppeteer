cmake_minimum_required(VERSION 3.11)

project(Puppeteer CXX)

set(CMAKE_CXX_STANDARD 14)

add_executable(Puppeteer main.cpp)

find_package(Boost 1.68.0 REQUIRED system)

target_include_directories(Puppeteer PUBLIC ${Boost_INCLUDE_DIR})
target_link_libraries(Puppeteer PUBLIC  ${Boost_LIBRARIES} )