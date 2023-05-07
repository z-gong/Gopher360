cmake_minimum_required(VERSION 3.17)
project(Gopher360)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_EXE_LINKER_FLAGS "-static")

include_directories(Gopher)

add_executable(Gopher360
        Gopher/ConfigFile.cpp
        Gopher/ConfigFile.h
        Gopher/Convert.h
        Gopher/CXBOXController.cpp
        Gopher/CXBOXController.h
        Gopher/Gopher.cpp
        Gopher/Gopher.h
        Gopher/main.cpp
        Gopher/resource.h)

target_link_libraries(Gopher360 Xinput)
