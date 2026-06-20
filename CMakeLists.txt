# Design Patterns - (c) 2026 Example Org - MIT License
# Author: Engineering Team <engineering@example.com>
cmake_minimum_required(VERSION 3.27)
project(cpp_example_design_patterns
        VERSION 1.0.0
        DESCRIPTION "Demonstracao de padroes de projeto isolando regras de negocio da infraestrutura."
        HOMEPAGE_URL "https://git.example.com/cpp-example-design-patterns"
        LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 20)
include_directories(include)

file(GLOB SOURCES src/*.cpp)
add_executable(app ${SOURCES})

enable_testing()
add_test(NAME unit COMMAND app)
