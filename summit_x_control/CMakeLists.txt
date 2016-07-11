cmake_minimum_required(VERSION 2.8.3)
project(summit_x_control)


find_package(catkin REQUIRED COMPONENTS 
	roslaunch 
	summit_xl_pad 
	summit_x_description
	ros_controllers
	ros_control
	robot_state_publisher
)

catkin_package()

include_directories(${catkin_INCLUDE_DIRS})

install(
  DIRECTORY launch config
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)
