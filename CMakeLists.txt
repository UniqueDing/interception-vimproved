cmake_minimum_required(VERSION 3.0)

project(interception-vimproved)

add_executable(interception-vimproved interception-vimproved.cpp)
target_compile_options(interception-vimproved PRIVATE -Wall -Wextra -std=c++17)
target_link_libraries(interception-vimproved yaml-cpp)

install(TARGETS interception-vimproved RUNTIME DESTINATION bin)
