------------------------
  TURTLE ROBOT PACKAGE
------------------------
v 0.1.0
Author: Florencia Grosso
Date: 02/05/2017
------------------------

Information on this package:

This package provides a node, turtle_robot, which publishes on the turlstim cmd_vel topic and makes the sim node draw a figure at a given speed. 

The drawer receives the name of the file containing the figure to sketch and the speed of the turtle as ROS parameters in the launch file. The default values for these parameters are: xspeed = 5, figure_file = star.csv .To change this settings, go to the turtle_robot.launch file and edit the speed value and the name of the figure file. You can find other figures in the ~/turtle_robot/figures folder .


I. How to BUILD it:

1. In a new terminal, go to your catkin workspace:

$ ~/<your catkin workspace>/src

2. Now clone this folder:

# [In your catkin workspace/src]
$ git clone https://github.com/FlorGrosso/TechnicalChallenge_TR

2. Move back to your catkin workspace folder and run the catkin_make command to build the project as follows:

$ cd ~/<your catkin workspace>

$ catkin_make 

3. Don't forget to source the environment setup files:

$ source ~/<your catkin workspace>/devel/setup.bash


II. How to RUN it:

1. Run the launch file with the following command:

$roslaunch turtle_robot turtle_robot.launch 


If you run the launch file in a new terminal and you get an error message indicating that the package 'turtle_robot' is not found, you will need to source the setup files (step 3 of how to BUILD) once again.

