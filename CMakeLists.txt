cmake_minimum_required(VERSION 3.0)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -fPIC")

project(ImGui)

add_library(imgui imconfig.h imgui.h imgui_internal.h imstb_rectpack.h imstb_textedit.h imstb_truetype.h imgui.cpp imgui_demo.cpp imgui_draw.cpp imgui_widgets.cpp)
target_include_directories(imgui PUBLIC .)
