cmake_minimum_required(VERSION 3.0.2)
project(planning)
find_package(catkin REQUIRED COMPONENTS roscpp)
include_directories(
 ${catkin_INCLUDE_DIRS}
)
set (CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -g ")
set (CMAKE_VERBOSE_MAKEFILE ON)
#
catkin_package()
add_executable(locpl src/test.cpp)
target_link_libraries(locpl ${catkin_LIBRARIES})

#add_executable(globpl src/glo.cpp)
#target_link_libraries(globpl ${catkin_LIBRARIES})
