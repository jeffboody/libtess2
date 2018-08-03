cmake_minimum_required(VERSION 3.4.1)

# Compiler options
add_compile_options(-Wall)

# Submodule library
add_library(tess2
            STATIC

            # Source
            Source/bucketalloc.c
            Source/dict.c
            Source/geom.c
            Source/mesh.c
            Source/priorityq.c
            Source/sweep.c
            Source/tess.c)

# Linking
target_link_libraries(tess2)
