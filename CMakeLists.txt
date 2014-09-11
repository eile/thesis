project(Eyescale)
cmake_minimum_required(VERSION 2.8)

option(BUILDYARD_DISABLED "Disable bootstrapping using Buildyard" ON)
include(${PROJECT_SOURCE_DIR}/CMake/GitExternal.cmake)
include(${PROJECT_SOURCE_DIR}/CMake/common/SubProject.cmake)

add_git_subproject(vmmlib https://github.com/Eyescale/vmmlib.git master)
add_git_subproject(Lunchbox https://github.com/Eyescale/Lunchbox.git master)
add_git_subproject(Collage https://github.com/Eyescale/Collage.git master)
add_git_subproject(hwsd https://github.com/Eyescale/hwsd.git master)
add_git_subproject(GLStats https://github.com/Eyescale/GLStats.git master)
add_git_subproject(Equalizer https://github.com/Eyescale/Equalizer.git master)
