# remap_joy 
Remapping of the joy_node topic in ROS2 for the use of different joysticks in multiple systems. This way it's possible to operate our custom [marum_minirov](https://github.com/MARUM-MUtTI/marum_minirov.git) and on the other hand our [underwater_bodennode](https://github.com/MARUM-MUtTI/underwater_bodennode.git) through its respective surface computer, where each system has its own joystick.

## Installation
- Clone the repository and compile it:
```
source /opt/ros/galactic/setup.bash
mkdir -p ~/ros2_ws/src
cd ~/ros2_ws/src
git clone https://github.com/MARUM-MUtTI/remap_joy.git
cd ..
colcon build
```

## Usage
- It only remains to launch the node:
```
source install/local_setup.bash
ros2 launch remap_joy remap_joy.launch.py topic_name:='name'
```
