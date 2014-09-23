project(Thesis)
cmake_minimum_required(VERSION 2.8)

option(BUILDYARD_DISABLED "Disable bootstrapping using Buildyard" ON)
include(${PROJECT_SOURCE_DIR}/CMake/GitExternal.cmake)
include(${PROJECT_SOURCE_DIR}/CMake/common/SubProject.cmake)

# external dependencies
add_git_subproject(FlatBuffers https://github.com/eile/flatbuffers.git master)
add_subdirectory(ITK-config)

# Eyescale dependencies
add_git_subproject(vmmlib https://github.com/eile/vmmlib.git master)
add_git_subproject(Lunchbox https://github.com/eile/Lunchbox.git master)
add_git_subproject(Collage https://github.com/eile/Collage.git master)
add_git_subproject(hwsd https://github.com/eile/hwsd.git master)
add_git_subproject(GLStats https://github.com/eile/GLStats.git master)
add_git_subproject(Equalizer https://github.com/eile/Equalizer.git master)

# BlueBrain dependencies
add_git_subproject(zeq https://github.com/eile/zeq.git master)
add_git_subproject(Fivox ssh://bbpcode.epfl.ch/viz/Fivox Fivox)
