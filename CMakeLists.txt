cmake_minimum_required(VERSION 3.10)

project(QuantStartExamples)

set(CMAKE_CXX_STANDARD 17)

add_executable(asian_option_mc src/main.cpp src/asian.cpp src/payoff.cpp)
target_include_directories(asian_option_mc PRIVATE include)

add_executable(european_option_mc src/european_option_mc.cpp)
target_include_directories(european_option_mc PRIVATE include)
