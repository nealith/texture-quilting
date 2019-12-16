CMAKE_MINIMUM_REQUIRED(VERSION 2.8)

PROJECT(TextureQuilting)

find_package( OpenCV REQUIRED )
include_directories(${OpenCV_INCLUDE_DIRS} ${TextureQuilting_SOURCE_DIR}/includes)
file(GLOB SOURCES
    ./src/*.cpp
)

add_compile_options("-g" "-O2")

add_library(${PROJECT_NAME} STATIC ${SOURCES})
ADD_EXECUTABLE(testGeneration testGeneration.cpp)
ADD_EXECUTABLE(testTransfert testTransfert.cpp)

target_link_libraries( ${PROJECT_NAME} ${OpenCV_LIBS} "-lm")
target_link_libraries( testGeneration ${PROJECT_NAME} "-lm")
target_link_libraries( testTransfert ${PROJECT_NAME} "-lm")
