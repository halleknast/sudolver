PROJECT(sudolver)
CMAKE_MINIMUM_REQUIRED(VERSION 3.1)

FILE(GLOB SRC ${CMAKE_CURRENT_SOURCE_DIR}/src/*.c)
SET(ARGTABLE ${CMAKE_CURRENT_SOURCE_DIR}/lib/argtable3/argtable3.c)

ADD_EXECUTABLE(${PROJECT_NAME} ${SRC} ${ARGTABLE})

SET_PROPERTY(TARGET ${PROJECT_NAME} PROPERTY C_STANDARD 99)
