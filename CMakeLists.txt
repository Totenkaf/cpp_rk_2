# Copyright 2022 by Artem Ustsov

# ==============================================================================
# I | General project settings
# ==============================================================================
cmake_minimum_required(VERSION 3.8)
set(project_name ping_pong)
project(${project_name})


set(CMAKE_CXX_STANDARD 20)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -pthread -Wall -Wextra -Wpedantic -Werror")

# ==============================================================================
# II | Preinstall settings
# ==============================================================================


# ------------------------------------------------------------------------------
# Executable Main
# ------------------------------------------------------------------------------

add_executable(${PROJECT_NAME} rk.cpp)
