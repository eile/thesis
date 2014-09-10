project(Eyescale)
cmake_minimum_required(VERSION 2.8)

include(${PROJECT_SOURCE_DIR}/CMake/GitExternal.cmake)
include(${PROJECT_SOURCE_DIR}/CMake/common/SubProject.cmake)

add_git_subproject(Lunchbox https://github.com/Eyescale/Lunchbox.git master)
add_git_subproject(Collage https://github.com/Eyescale/Collage.git master)
add_git_subproject(Equalizer https://github.com/Eyescale/Equalizer.git master)
