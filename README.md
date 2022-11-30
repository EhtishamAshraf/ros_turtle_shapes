# ROS Turtle Shapes

This repository contains the code to draw shapes (i.e., square, rectangle, triangle, square) and reaching a specific goal with turtlesim.


# Create Ros Workspace
Open shell and execute the following commands:
```bash
mkdir my_ros_ws
```
```bash
cd my_ros_ws
```
```bash
mkdir src
```
Run the below command in root folder of the workspace
```bash
catkin_make 
```
Navigate to the src folder and create your package
```bash
cd src 
```
```bash
catkin_create_pkg turtlebot_controller std_msgs roscpp rospy
```
```bash
Navigate to the package and inside the src folder, clone this repository
cd turtlebot_controller/src
```
# Download the Code
```bash
sudo apt-get update
```
```bash
sudo apt-get install git
```
```bash
https://github.com/EhtishamAshraf/ros_turtle-shapes.git
```
Run the command below, to make the python file executable. Run the command in the src folder (where the python file is present)
```bash
chmod +x turtle_shapes.py
```
roscore must be running in order for ROS nodes to communicate. Open a new terminal and run roscore with this command:
```bash
roscore &
```
Press Enter and write the command below to open turtlesim : (Assuming that turtlesim is already installed!) 
```bash
rosrun turtlesim turtlesim_node 
```
Open a new shell windown and run the following the commands in sequence:
```bash
catkin_make
```
```bash
source devel/setup.bash
```
```bash
rosrun turtlebot_controller turtle_shapes.py
```
