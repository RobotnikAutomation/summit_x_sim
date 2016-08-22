summit_x_sim
=============

Packages for the simulation of the Summit-X

<h2>summit_x_sim_bringup</h2>

launch files that launch the complete simulation of the robot

To start the simulation:
`roslaunch summit_x_sim_bringup summit_x_complete.launch`

<h2>summit_x_gazebo</h2>

launch files and world files to start the models in gazebo

<h2>summit_x_control</h2>

<p>This package contains the launch and configuration files to spawn the joint controllers with the ROS controller_manager.

<h2>summit_x_robot_control</h2>

<p>control the robot joints in all kinematic configurations, publishes odom topic and, if configured, also tf odom to base_link. Usually takes as input joystick commands and generates as outputs references for the gazebo controllers defined in summit_xl_control. This package permits an alternative way to control the robot motion (4 motorwheels) that by default is carried on by the Gazebo plugin (skid-steer). In the default configuration this package only controls the pan-tilt camera joints.

When used as main controller of the simulated robot, this node also computes the odometry of the robot using the joint movements and a IMU and publish this odometry to /odom. The node has a flag in the yaml files that forces the publication or not of the odom->base_footprint frames, needed by the localization and mapping algorithms.
</p>


