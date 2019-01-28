cmake_minimum_required(VERSION 3.13)
project(AirobTest)

set(CMAKE_CXX_STANDARD 14)

include_directories(src)

add_executable(AirobTest
        src/astar_algoirthm.cpp
        src/astar_algorithm.h
        src/astar_MapConfirm.cpp
        src/astar_MapConfirm.h
        src/CleanPlaner.cpp
        src/CleanPlaner.h
        src/CommHelper.cpp
        src/CommHelper.h
        src/inifile.c
        src/inifile.h
        src/main.cpp
        src/main.h
        src/MapDealer.cpp
        src/MapDealer.h
        src/TCPClient.cpp
        src/TCPClient.h
        src/unit.cpp
        src/unit.h)

find_package(Threads REQUIRED)
target_link_libraries(AirobTest Threads::Threads)