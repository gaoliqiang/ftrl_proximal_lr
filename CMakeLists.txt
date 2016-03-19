cmake_minimum_required(VERSION 3.3)
project(ftrl_proximal_lr)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")
add_subdirectory(src)

add_executable(ftrl_train src/ftrl_train.cpp)
target_link_libraries(ftrl_train stopwatch)

add_executable(ftrl_predict src/ftrl_predict.cpp)
target_link_libraries(ftrl_predict stopwatch)