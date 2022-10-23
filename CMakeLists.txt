cmake_minimum_required (VERSION 3.2)
project (HELLO)

set(wxBUILD_SHARED OFF)
add_subdirectory(libs/wxWidgets)

include_directories(src)

file (GLOB_RECURSE MY_APP CONFIGURE_DEPENDS
    src/*.h
    src/*.cpp
)

add_executable(hello ${MY_APP})
target_link_libraries(hello wx::net wx::core wx::base)