# SK26: ROS 2 Jazzy and Gazebo simulation

## About the project:
Control a TurtleBot3 (Burger model) in a ROS2 Jazzy and Gazebo simulation environment to autonomously execute a precise square-driving maneuver.

## What will you gain from it?
You will learn some basics of ROS 2 Jazzy and Gazebo Simulation.

## Setup your environment
To start the project you need to install Ubuntu Linux (version 24.04) on your computer. There's plenty of tutorials to help you.

Then you need to install ROS 2 Jazzy environment and Gazebo Simulator. Here's a full guide + first program you can run: https://automaticaddison.com/how-to-install-ros-2-jazzy/

After successful installation, you can build your ros2 workspace and package. This will be your place to store the code. Here's a tutorial: https://automaticaddison.com/how-to-create-a-ros-2-package-jazzy/ (this is also in the tutorial in the ROS2 Jazzy Tutorial section)

Then clone this repository to your src folder. 
You can do it via https or SSH. The second option is recomended. For that create your SSH key, add it to your GitHub account and use git clone, copy the url for https or SSH.

After that, install a packet of 3d model robot with lidar:
```markdown
sudo apt update
sudo apt install ros-jazzy-turtlebot3*
```

Now you are ready to start working on the code. Use Python for that.
I recommend to learn from the official documentation of ROS2 or watch tutorials on youtube. Learn how publishers and subscribers work, and you're good to go! 

## How to upload your code there?
Before uploading, please name your script SK26_YourName_YourSurname.
Go into your scr folder in terminal, then 
```markdown
git add .
git commit -m "[write what you did]"
git push
```
You can also use git status command to check if there where some changes in repositoty. If there where, a git pull command will update your local copy on your computer.

## Tips
To see your robot in Gazebo, open terminal and type:
```markdown
export TURTLEBOT3_MODEL=burger
ros2 launch turtlebot3_gazebo empty_world.launch.py use_sim_time:=true
```
I recommend to set the robot in motion, generally experiment with Gazebo (not obligatory to finish the project)

## ROS Topics
The project relies on standard ROS 2 message types and interfaces for the TurtleBot3 simulation:

* **/scan** (`sensor_msgs/msg/LaserScan`): Subscribed to receive raw laser distance data from the robot's Lidar for obstacle detection.
* **/cmd_vel** (`geometry_msgs/msg/Twist`): Published to control linear and angular velocities of the robot.
* **/obstacle_detected** (`std_msgs/msg/String`): Custom topic used to publish alert notifications when an obstacle is detected within the safety threshold.

## ROS2 Jazzy Tutorial:
https://www.youtube.com/watch?v=DM77KkIJsik&list=PLNWNEEf8BvG64FVZT4IdieI1PuYnHkUrt&index=1 - shows you basics of ROS2 + simulations in Gazebo


## Deadline
You have time till 16th of December. Good luck!
