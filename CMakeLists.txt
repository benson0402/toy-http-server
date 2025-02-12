cmake_minimum_required(VERSION 3.20)
project(ToyHTTPServer LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 23)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

set(CMAKE_TOOLCHAIN_FILE "${CMAKE_SOURCE_DIR}/vcpkg/scripts/buildsystems/vcpkg.cmake" CACHE STRING "")

find_package(Boost REQUIRED COMPONENTS asio beast)

add_executable(ToyHTTPServer src/main.cpp)

target_link_libraries(ToyHTTPServer PRIVATE Boost::asio Boost::beast)

