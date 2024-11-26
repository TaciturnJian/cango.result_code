cmake_minimum_required(VERSION 3.21)

project(cango.result_code)

add_library(cango_result_code INTERFACE)
add_library(cango::utility::result_code ALIAS cango_result_code)
target_include_directories(cango_result_code INTERFACE include)
set_target_properties(cango_result_code PROPERTIES CXX_STANDARD 20)

if (MSVC)
    add_compile_options(/utf-8)
endif()

if (PROJECT_IS_TOP_LEVEL)
    # TODO: Add tests
endif()
