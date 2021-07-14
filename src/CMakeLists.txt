cmake_minimum_required(VERSION 3.10)

project(main)

find_package( Boost REQUIRED COMPONENTS filesystem )
include_directories( ${Boost_INCLUDE_DIRS} )

# Set sources to be compiled
set( SOURCES main.cpp)
add_executable( main ${SOURCES})
target_link_libraries(main  ${Boost_FILESYSTEM_LIBRARY})