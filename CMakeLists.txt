cmake_minimum_required(VERSION 3.10)

project(QuantStartExamples)

set(CMAKE_CXX_STANDARD 17)

add_executable(asian_option_mc src/main_asian_option_mc.cpp
                                    src/asian.cpp
                                    src/payoff.cpp)
target_include_directories(asian_option_mc PRIVATE include)

add_executable(european_option_bs src/main_european_option_bs.cpp)
target_include_directories(european_option_bs PRIVATE include)

add_executable(european_option_mc src/main_european_option_mc.cpp)
target_include_directories(european_option_mc PRIVATE include)

add_executable(linear_congruent_generator src/main_lin_con_gen.cpp
                                          src/lin_con_gen.cpp)
target_include_directories(linear_congruent_generator PRIVATE include)

add_executable(standard_distribution src/main_statistics.cpp
                                     src/statistics.cpp)
target_include_directories(standard_distribution PRIVATE include)

add_executable(correlated_stocks src/main_correlation.cpp
                                src/correlated_snd.cpp
                                src/statistics.cpp)
target_include_directories(correlated_stocks PRIVATE include)

add_executable(heston src/main_heston.cpp
                      src/heston_mc.cpp
                      src/option.cpp
                      src/payoff.cpp
                      src/statistics.cpp
                      src/correlated_snd.cpp)
target_include_directories(heston PRIVATE include)
