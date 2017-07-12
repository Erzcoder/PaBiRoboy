# PaBiRoboy
this repo combines all packages for dancing PaBi

# dependencies
* [ROS kinetic](http://wiki.ros.org/kinetic/Installation/Ubuntu)
* sudo apt install ros-kinetic-aruco-detect ros-kinetic-qt-build
* sudo apt install gcc-arm-linux-gnueabihf g++-arm-linux-gnueabihf
* [librealsense](https://github.com/IntelRealSense/librealsense)

# build
```
!#/bin/bash
cd /path/to/PaBiRoboy
catkin_make
```

# run it
```
!#/bin/bash
cd /path/to/PaBiRoboy
sudo -s # you need to be root for the powerlink stack (ie communication with pabi) to be working
source devel/setup.bash
roslaunch roboy_interface PaBi_dance.launch
```
