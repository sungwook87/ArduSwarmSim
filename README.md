# ArduSwarmSim
## Ardupilot based UAV Swarm + Gazebo simulator
### This is a instruction for using KETI GCS + nCube_MUV + Ardupilot + Gazebo

<img src="https://github.com/HKUST-Aerial-Robotics/ArduSwarmSim/gcs.png" width = 55% height = 55%/>



## 1. Prerequisites
### 1.1 **Ubuntu** and **ROS**
Ubuntu 64-bit 18.04.
ROS Melodic. [ROS Installation](http://wiki.ros.org/ROS/Installation)


### 1.2. **Gazebo 8 or 9**
Make sure you run Gazebo at leat once.
```
    gazebo --verbose /usr/share/gazebo-8/worlds/iris_arducopter_demo.world
```


### 1.3. **Install ardupilot_gazebo plugin**
[ardupilot_gazebo](https://github.com/SwiftGust/ardupilot_gazebo)




## 2. Build VINS-Fusion
Clone the repository and catkin_make:
```
    cd ~/catkin_ws/src
    git clone https://github.com/HKUST-Aerial-Robotics/VINS-Fusion.git
    cd ../
    catkin_make
    source ~/catkin_ws/devel/setup.bash
```
