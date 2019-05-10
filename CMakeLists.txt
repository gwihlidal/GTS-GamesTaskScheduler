cmake_minimum_required(VERSION 3.14)
set(CMAKE_CXX_STANDARD 11)

file(GLOB_RECURSE HEADERS ./source/gts/source/*.h)
file(GLOB_RECURSE SOURCES ./source/gts/source/*.cpp)

include_directories("./source/gts/include")

#file(GLOB SOURCE_FILES ${PROJECT_SOURCE_DIR}/source/gts/source/*.cpp)

ADD_LIBRARY(gts STATIC
	${HEADERS}
	${SOURCES}
)