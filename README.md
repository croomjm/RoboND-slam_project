# RoboND-slam-project

## Project Summary

I completed this project as part of my [Udacity Robotics Software Engineer Nanodegree](https://confirm.udacity.com/AQCTW57M). As part of the project, I created my own custom Roomba-like robot in ROS using XML robot description files and a custom STL model. The robot incorporated a simulated wheel encoders and an RGBD camera. Using the [RTAB-Map](http://introlab.github.io/rtabmap/) library, I mapped simulated rooms within ROS and localized the robot within them. Details of my approach can be found [here](./SLAM_project_report.pdf). An academic-style report rather than a detailed markdown readme was required as part of the project.

Videos of successful completion of the course can be found [here](https://youtu.be/2CB-RQJTMQY) and [here](https://youtu.be/TnGkOjb4IYg).

## Downloading and Running the Software

This repository contains code for the Udacity Robotics Nanodegree SLAM project. It is meant to run on a dedicated workspace hosted by Udacity, but you may also be able to make it work in linux ROS on another platform with appropriate dependencies installed.

Launch the environment as follows from within the catkin workspace:
`roslaunch slam_project ultra_udacity_world.launch`

This command can be launched with an additional option to launch in any world as desired:
`world:=[path to .world file]`

In a separate terminal window, launch the robot teleop program to navigate around the scene:
`roslaunch slam_project teleop.launch`


The primary launch file has been modified to concurrently launch the [RTAB-Map](http://wiki.ros.org/rtabmap_ros) SLAM node as well.

