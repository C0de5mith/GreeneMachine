# GreeneMachine
Autonomous vehicles repository for code sharing

### Jetpack
If the jetson does not already have ubuntu 16 on it, flash it to the jetson using [NVIDIA JetPack](https://developer.nvidia.com/embedded/jetpack)

### ROS Setup
Install ROS on your jetson by following the directions on the [ROS Wiki](http://wiki.ros.org/kinetic/Installation/Ubuntu)

### Install ZED SDK
   [Sterio Labs Ros Integration](https://github.com/stereolabs/zed-ros-wrapper#stereolabs-zed-camera---ros-integration)
      -We used a 2.x version of the ros wrapper because the latest SDK version that had JetsonTX1 support was 2.8.5
      -Also a note worthy error ouucred that sl/Camera.hpp couldnt be found and this was because we had another wersion of zed sdk installed and then installed an older zed on top of it so it put all zed include headers into zed_previous(simple fix is to rename it to zed) in foler usr/local/zed
   
### Install ROS nodes
Install all needed nodes 
  -9Dof Razer IMU (http://wiki.ros.org/razor_imu_9dof)
  --Follow the guide on installing libs and boards for arduino ide for [9dof-razor-imu-m0](https://learn.sparkfun.com/tutorials/9dof-razor-imu-m0-hookup-guide)

### Daily Setup
Moniter
  -Plug in Moniter to power (not Jetson)
  -Connect HDMI to Jetson
USB-Hub
  -Connect USB hub to Jetson
  -Plug in keyboard and mouse
Power on Jetson
  -The first time powering up the jetson ubuntu must set up (https://tutorials.ubuntu.com/tutorial/tutorial-install-ubuntu-desktop#0)
Other Daily Procedures
  -plug in other devices you wish to configure into correct ports on jetson
