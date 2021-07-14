cmake_minimum_required(VERSION 3.10)

project(main)

find_package( Boost REQUIRED COMPONENTS regex )
include_directories( ${Boost_INCLUDE_DIRS} )

# Set sources to be compiled
set( SOURCES "main.cpp" )
add_executable( main ${SOURCES})
target_link_libraries(main ${Boost_PROGRAM_OPTIONS_LIBRARY} ${Boost_REGEX_LIBRARY})