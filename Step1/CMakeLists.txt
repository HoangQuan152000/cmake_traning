# CMakeList.txt : CMake project for 19092024, include source and define
# project specific logic here.
#
cmake_minimum_required (VERSION 3.8)

project (19092024 VERSION 1.0)
configure_file(TutorialConfig.h.in TutorialConfig.h)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED true)

# Add source to this proj".cpp"le.
add_executable (19092024 "tutorial.cpp")

# TODO: Add tests and install targets if needed.
target_include_directories(19092024 PUBLIC "${PROJECT_BINARY_DIR}")

