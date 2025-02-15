cmake_minimum_required(VERSION 3.30)
project(bankyron)

set(CMAKE_CXX_STANDARD 20)

include_directories(include)

set(SOURCES
    src/main.cpp
    src/User.cpp
)

set(HEADERS
    include/User.h
)

# Creăm executabilul cu toate sursele
add_executable(${PROJECT_NAME} ${SOURCES} ${HEADERS})
