# PaBiRoboy
this repo combines all packages for dancing PaBi

# dependencies
* [ROS kinetic](http://wiki.ros.org/kinetic/Installation/Ubuntu)
* sudo apt install ros-kinetic-aruco-detect ros-kinetic-qt-build
* sudo apt install gcc-arm-linux-gnueabihf g++-arm-linux-gnueabihf
* sudo apt install protobuf-compiler
* [librealsense](https://github.com/IntelRealSense/librealsense)
* [altera soc eds standard version](https://dl.altera.com/soceds/) for arm cross compilation

# build
```
!#/bin/bash
cd /path/to/PaBiRoboy
~/intelFPGA/17.0/embedded/embedded_command_shell.sh  # only necessary if you want to cross compile for arm
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
