#
# Skeleton CMake project file for libtess2
#
cmake_minimum_required(VERSION 2.8)

project (libtess2) 


set(LIBTESS2_SOURCES
    src/bucketalloc.c
    src/dict.c
    src/geom.c
    src/mesh.c
    src/priorityq.c
    src/sweep.c
    src/tess.c
)

INCLUDE_DIRECTORIES(${CMAKE_CURRENT_SOURCE_DIR}/src)
ADD_LIBRARY(tess2 ${LIBTESS2_SOURCES})