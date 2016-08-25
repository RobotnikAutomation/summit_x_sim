cmake_minimum_required(VERSION 2.8.3)
project(summit_x_sim_bringup)

find_package(catkin)
catkin_package()

install(
  DIRECTORY launch
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)

