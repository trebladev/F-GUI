cmake_minimum_required(VERSION 3.23)
project(F_GUI)

set(CMAKE_CXX_STANDARD 14)
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)

set(CMAKE_PREFIX_PATH "/home/xuan/Qt5.11.3/5.11.3/gcc_64/lib/cmake")

find_package(Qt5 COMPONENTS
        Core
        Gui
        Widgets
        REQUIRED)

add_executable(F_GUI main.cpp)
target_link_libraries(F_GUI
        Qt5::Core
        Qt5::Gui
        Qt5::Widgets
        )

