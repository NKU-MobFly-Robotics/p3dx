# Pioneer 3-DX Simulator
This repo contains the materials for Pioneer 3-DX mobile robot simulation in Gazebo. The original code comes from https://github.com/BruceChanJianLe/p3dx. Thanks go to CHAN JIAN LE.

## Requirements
```
sudo apt install ros-kinetic-gazebo-ros-control ros-kinetic-diff-drive-controller ros-kinetic-joint-state-controller ros-kinetic-robot-state-publisher
```

## Clone and build

Please create and initialize a ROS workspace. We assume that your workspace is named catkin_ ws. Then, run the following commands to clone this repo:
```
$ cd ~/catkin_ws/src
$ git clone https://github.com/NKU-MobFly-Robotics/p3dx.git
```
If you are using Ubuntu 16.04, please switch to the kinetic-devel branch:
```
$ git branch -a
$ git checkout kinetic-devel
```
You can use the following command to check the current git status
```
git status
```
Finally, build this repo
```
$ cd ~/catkin_ws/
$ catkin_make -DCMAKE_BUILD_TYPE=Release
```