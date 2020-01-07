cmake_minimum_required(VERSION 3.12)

project(vcpkg_test_k4a)

find_package(k4a CONFIG REQUIRED)

add_executable(test_vcpkg_k4a)
target_sources(test_vcpkg_k4a
  PRIVATE
    main.cpp
)
target_link_libraries(test_vcpkg_k4a
  PRIVATE
    k4a::k4a
)
