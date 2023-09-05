cmake_minimum_required(VERSION 3.5)

project (hello_headers)

# Create a sources variable with a link to all cpp files to compile
set(SOURCES
    src/Hello.cpp
    src/main.cpp
)

add_executable(hello_headers ${SOURCES})

target_include_directories(hello_headers
    PRIVATE
        ${PROJECT_SOURCE_DIR}/include
)
