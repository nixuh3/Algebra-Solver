cmake_minimum_required(VERSION 3.20)
project(Algebra-Solver LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

set(SOURCES
    src/Main.cpp
    src/Parser.cpp
    src/Solver.cpp
    src/Tokenizer.cpp
    src/Utils.cpp

    src/Parser.h
    src/Solver.h
    src/Tokenizer.h
    src/Utils.h
)

add_executable(${PROJECT_NAME} ${SOURCES})

# Match VS filters to directory structure on disk
source_group(TREE "${CMAKE_CURRENT_SOURCE_DIR}" FILES ${SOURCES})