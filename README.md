# RoboND-slam-project

This repository contains code for the Udacity Robotics Nanodegree SLAM project. It is meant to run on a dedicated workspace hosted by Udacity, but you may also be able to make it work in linux ROS on another platform with appropriate dependencies installed.

Launch the environment as follows from within the catkin workspace:
`roslaunch slam_project ultra_udacity_world.launch`

This command can be launched with an additional option to launch in any world as desired:
`world:=[path to .world file]`

In a separate terminal window, launch the robot teleop program to navigate around the scene:
`roslaunch slam_project teleop.launch`


The primary launch file has been modified to concurrently launch the [RTAB-Map](http://wiki.ros.org/rtabmap_ros) SLAM node as well.

Videos of successful completion of the course can be found [here](https://youtu.be/2CB-RQJTMQY) and [here](https://youtu.be/TnGkOjb4IYg).
