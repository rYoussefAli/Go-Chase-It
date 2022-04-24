# Go-Chase-It
###### Robotics project by ROS and Gazebo environment

## Contents
1. [Installation](#Installation)
2. [Motivation](#Motivation)
3. [Setup](#Setup)
4. [Use](#Use)
5. [License](#License)

## Installation
To run this project you should have [Gazebo environment](http://gazebosim.org/) and [ROS](https://www.ros.org/)

## Motivation
I create this project to practice my skills in Robotics Developing

## Setup
Before launching the project you should initialize a catkin workspace
```
$ mkdir -p catkin_ws/src
$ cd catkin_ws
$ catkin_init_workspace
```
Download this git repo, extract the folders and remove the master folder
```
$ git clone https://github.com/rYoussefAli/Go-Chase-It.git
$ cp -R Go-Chase-It/ball_chaser .
$ cp -R Go-Chase-It/my_robot .
$ rm -rf Go-Chase-It
```
Build the world
```
$ cd ..
$ catkin_make
```
Source the setup.bash and run the world
```
$ source devel/setup.bash
$ roslaunch my_robot world.launch
```
Now you have the wrld and the robot<br><br>
To make it chase the ball: <br>
Open another terminal and type
```
$ cd catkin_ws
$ source devel/setup.bash
$ roslaunch ball_chaser ball_chaser.launch
```
And that's it, now you have a ball-chaser robot!

## Use
It is completely simple, just run the world, move the ball, and the robot will do the rest.

## License
This project is under [GNU License](https://github.com/YoussefAli99/Go-Chase-It/blob/master/LICENSE)
