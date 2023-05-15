cmake_minimum_required(VERSION 3.14)
project(st-ui)

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
set(CMAKE_CXX_STANDARD 14)


find_package(Qt5
	REQUIRED COMPONENTS
	Core Gui Network Widgets Multimedia MultimediaWidgets)
  
add_subdirectory(src)
