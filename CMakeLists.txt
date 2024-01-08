CMAKE_MINIMUM_REQUIRED (VERSION 3.6)

PROJECT (nasbench)
include_directories(common)
file(GLOB_RECURSE SOURCE_FILES common/*.c)

add_executable(bt BT/bt.c ${SOURCE_FILES})
add_executable(is IS/is.c ${SOURCE_FILES})
add_executable(lu LU/lu.c ${SOURCE_FILES})
add_executable(sp SP/sp.c ${SOURCE_FILES})
add_executable(cg CG/cg.c ${SOURCE_FILES})
add_executable(ep EP/ep.c ${SOURCE_FILES})
add_executable(ft FT/ft.c ${SOURCE_FILES})
add_executable(mg MG/mg.c ${SOURCE_FILES})