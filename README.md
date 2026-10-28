# SK26: ROS 2 Jazzy and Gazebo simulation

## About the project:
Control a TurtleBot3 (Burger model) in a ROS2 Jazzy and Gazebo simulation environment to autonomously execute a precise square-driving maneuver.

## What will you gain from it?
You will learn some basics of ROS 2 Jazzy and Gazebo Simulation.

## Setup your environment
To start the project you need to install Ubuntu Linux on your computer. There's plenty of tutorials to help you.

Then you need to install ROS 2 Jazzy environment and Gazebo Simulator. Here's a full guide + first program you can run: https://automaticaddison.com/how-to-install-ros-2-jazzy/

After successful installation, you can build your ros2 workspace. This will be your place to store the code. Here's a tutorial: https://industrial-training-master.readthedocs.io/en/foxy/_source/session1/ros2/1-Create-ROS-Workspace.html

Then clone this repository to your src folder. 
You can do it via https or SSH. The second option is recomended. For that create your SSH key, add it to your GitHub account and use git clone, copy the url for https or SSH.

After that, install a packet of 3d model robot with lidar:
```markdown
sudo apt update
sudo apt install ros-jazzy-turtlebot3*
```

Now you are ready to start working on the code.
I recommend to learn from the official documentation of ROS2 or watch tutorials on youtube. Learn how publishers and subscribers work, and you're good to go! 

## How to upload your code there?
Go into your scr folder in terminal, then 
```markdown
git add .
git commit -m "comment"
git push
```
You can also use git status command to check if there where some changes in repositoty. If there where, a git pull command will update your local copy on your computer.

You have time till 16th of December. Good luck!







----------- smth
export TURTLEBOT3_MODEL=burger
ros2 launch turtlebot3_gazebo empty_world.launch.py use_sim_time:=true

dostaw sobie przedmiot. JESLI DZIALA TO WYLACZ. POTEM WROCIMY.

potem zbuduj rosowe srodowisko w ktorym bedizesz pracowac. 



potem na githuba
