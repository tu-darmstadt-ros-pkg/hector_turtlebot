cmake_minimum_required(VERSION 2.8.3)
project(hector_turtlebot_scan_filter)

find_package(catkin REQUIRED COMPONENTS roscpp sensor_msgs)

catkin_package(
#  INCLUDE_DIRS include
#  LIBRARIES challenge_master
#  CATKIN_DEPENDS challenge_msgs
#  DEPENDS system_lib
)

include_directories(include ${catkin_INCLUDE_DIRS} ${Boost_INCLUDE_DIRS})


## Declare a cpp executable
add_executable(hector_turtlebot_scan_filter src/hector_turtlebot_scan_filter.cpp)

## Specify libraries to link a library or executable target against
target_link_libraries(hector_turtlebot_scan_filter ${catkin_LIBRARIES})
