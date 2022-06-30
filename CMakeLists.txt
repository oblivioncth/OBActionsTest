cmake_minimum_required(VERSION 3.21.1)

# set the project name
project(Test)

# test doxygen
find_package(Doxygen 1.9.4
			 COMPONENTS dot
			 OPTIONAL_COMPONENTS mscgen dia
)

# add the executable
add_executable(test_exe main.cpp)