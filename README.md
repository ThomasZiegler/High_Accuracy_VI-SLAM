## High Accuracy Visual Inertial SLAM for Autonomous Navigation of small UAVs
### Overview
This repositry contains an adpated version of the VINS-Mono [1] SLAM system. The adaption reduce the computational demand of the system, allowing the system to run in real-time on e.g. a UP-Board. The accuracy is slightly decreased compared to the default implementation of VINS-Mono.

### Installation
This repo can directly be used as a ROS workspace. 

First Update the needed ROS modules
```
git submodule init
git submodule update
```
Then build the ROS modules
```
source /opt/ros/kinetic/setup.bash
catkin build catkin_simple
source devel/setup.bash
catkin build gflags_catkin
catkin build glog_catkin
catkin build ceres_catkin
catkin build
source devel/setup.bash
```


### References
[1] T. Qin, P. Li, and S. Shen, “VINS-Mono: A Robust and Versatile Monocular Visual-Inertial State Estimator,” CoRR, vol. abs/1708.0, pp. 1–17, 2017.
