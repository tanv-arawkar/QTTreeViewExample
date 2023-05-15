set (CMAKE_AUTOMOC ON)

add_library(app
	treemodel.cpp
	treeitem.cpp
	treemodel.h
	treeitem.h
	)

include_directories(${CMAKE_CURRENT_BINARY_DIR})

target_link_libraries(app
	Qt5::Gui
	Qt5::Core
	Qt5::Multimedia
	Qt5::MultimediaWidgets
	)

add_executable(ui
	main.cpp
	)

target_link_libraries(ui
	app
	)

install (TARGETS ui DESTINATION bin)
