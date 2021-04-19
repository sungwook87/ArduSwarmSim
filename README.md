# ArduSwarmSim
## Ardupilot based UAV Swarm + Gazebo simulator
### This is an instruction for using KETI GCS + nCube_MUV + Ardupilot + Gazebo
### This is for Non-ROS users

![ui](./img/gcs.png)

### Web GCS by [Autonomous IoT Research Center @ KETI](https://github.com/IoTKETI)



## 1. Prerequisites
1.1 **Ubuntu** and **ROS**

Ubuntu 64-bit 18.04., ROS Melodic. [ROS Installation](http://wiki.ros.org/ROS/Installation) (Not essential)


1.2 **ardupilot**

Follow the instructions below:

[ardupilot](https://github.com/ArduPilot/ardupilot)


1.3. **Install ardupilot_gazebo plugin**

Follow the instructions below:

[ardupilot_gazebo](https://github.com/SwiftGust/ardupilot_gazebo)


1.4. **Gazebo 8 or 9**

Make sure you run Gazebo at leat once.
```
    gazebo --verbose iris_arducopter_demo.world
```

1.5 **Modify the model & world files**

For multi-UAVs, we need to edit the model.sdf and world.world files.
```
    cd ~/path_to_[ardupilot_gazebo]/models/iris_with_standoffs_demo
    gedit model.sdf
```
Find "arducopter_plugin", and edit as shown in below Figure:

![ui](./img/model_sdf.png)
