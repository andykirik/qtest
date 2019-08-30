cmake_minimum_required(VERSION 3.5)

project(QTestApp
	VERSION 1.0.0
	LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 14)

find_package(Qt5 COMPONENTS Widgets REQUIRED)

set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)

if(CMAKE_VERSION VERSION_LESS "3.7.0")
    set(CMAKE_INCLUDE_CURRENT_DIR ON)
endif()

add_executable(QTestApp src/qtest.cpp)

target_link_libraries (QTestApp Qt5::Widgets)

