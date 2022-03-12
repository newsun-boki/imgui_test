cmake_minimum_required(VERSION 3.10)
project(imgui_test)

set(CMAKE_CXX_STANDARD 17)

# include_directories(gl3w)
include_directories(imgui)

add_executable(imgui_test
        # gl3w/GL/gl3w.c
        imgui/imgui.cpp
        imgui/imgui_demo.cpp
        imgui/imgui_draw.cpp
        imgui/imgui_impl_glfw.cpp
        imgui/imgui_impl_opengl3.cpp
        imgui/imgui_tables.cpp
        imgui/imgui_widgets.cpp
        main.cpp)

target_link_libraries(${PROJECT_NAME} GL GLU glfw3 X11 Xxf86vm Xrandr pthread Xi dl Xinerama Xcursor)
