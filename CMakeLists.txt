cmake_minimum_required(VERSION 3.10)

project(sp_lab4)

add_library(calculator STATIC calculator.c)

add_executable(calculator_app main.c)
target_link_libraries(calculator_app PRIVATE calculator)
