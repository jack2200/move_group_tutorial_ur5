# MoveIt! MoveGroup tutorial for UR5 (python interface)

Adaptation of [MoveIt! MoveGroup tutorial for Panda](https://github.com/ros-planning/moveit_tutorials/blob/kinetic-devel/doc/move_group_python_interface/)

## Installation

Need to use fixed URDF/SRDF universal_robotics package

``` 
mkdir -p ur5_ws/src && cd ur5_ws/src
git clone https://github.com/vfdev-5/universal_robot
git clone https://github.com/vfdev-5/move_group_tutorial_ur5.git
cd ../ & catkin_make
```

other dependencies (e.g if `moveit_commander` is not found):
```
sudo apt-get install ros-kinetic-moveit
```

## Usage:

Terminal 1
```
cd ur5_ws && source devel/setup.bash
roslaunch ur5_moveit_config demo.launch limited:=true
```

Terminal 2
```
cd ur5_ws && source devel/setup.bash
python src/move_group_tutorial_ur5/src/move_group_tutorial_ur5.py
```
