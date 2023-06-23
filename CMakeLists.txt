# basic root CMakeLists.txt file
cmake_minimum_required(VERSION 3.12)
project(test)

# Set C++ standard
set(CMAKE_CXX_STANDARD 11)

# Add your source files
set(SOURCES
    file1.c
    file2.c
    file3.c
)


# Create the executable
add_executable(${PROJECT_NAME} ${SOURCES} ${HEADERS})

# Specify include directories
target_include_directories(${PROJECT_NAME}
    PRIVATE include
)
