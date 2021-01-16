project(bsdgrep C)

set(SOURCES binary.c file.c grep.c mmfile.c queue.c util.c)
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wall -DNOZ=1")
set(CMAKE_EXE_LINKER_FLAGS "${CMAKE_EXE_LINKER_FLAGS} -lz" )

add_executable(bsdgrep ${SOURCES})
