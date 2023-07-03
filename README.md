# Pioneer 3-DX Simulator
This repo contains the materials for Pioneer 3-DX mobile robot simulation in Gazebo. The original code comes from https://github.com/BruceChanJianLe/p3dx. Thanks go to CHAN JIAN LE.

## Requirements
The ROS packages of gazebo_ros_control, diff_drive_controller, joint_state_controller, and robot_state_publisher are required.

For example, you can install these requirements on Ubuntu 20.04 by the following command:
```
sudo apt install ros-noetic-gazebo-ros-control ros-noetic-diff-drive-controller ros-noetic-joint-state-controller ros-noetic-robot-state-publisher
```

## Clone and build

Please create and initialize a ROS workspace. We assume that your workspace is named catkin_ws. Then, run the following commands to clone this repo:
```
$ cd ~/catkin_ws/src
$ git clone https://github.com/NKU-MobFly-Robotics/p3dx.git
```
If you are using Ubuntu 16.04/18.04, please switch to the kinetic/melodic-devel branch:
```
$ git branch -a
$ git checkout kinetic-devel  # for Ubuntu 16.04
$ git checkout melodic-devel  # for Ubuntu 18.04
```
You can use the following command to check the current git status:
```
git status
```
Finally, build this repo by the following commands:
```
$ cd ~/catkin_ws/
$ catkin_make -DCMAKE_BUILD_TYPE=Release
