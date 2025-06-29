cmake_minimum_required(VERSION 3.10)

project(QuantStartExamples)

set(CMAKE_CXX_STANDARD 17)

add_executable(asian_option_mc src/main.cpp src/asian.cpp src/payoff.cpp)
target_include_directories(asian_option_mc PRIVATE include)

add_executable(european_option_mc src/european_option_mc.cpp)
target_include_directories(european_option_mc PRIVATE include)

add_executable(linear_congruent_generator src/main_lin_con_gen.cpp src/lin_con_gen.cpp)
target_include_directories(linear_congruent_generator PRIVATE include)

add_executable(main_statistics src/main_statistics.cpp src/statistics.cpp)
target_include_directories(main_statistics PRIVATE include)

add_executable(main_correlation src/main_correlation.cpp src/correlated_snd.cpp src/statistics.cpp)
target_include_directories(main_correlation PRIVATE include)
