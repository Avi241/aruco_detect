# About  #
This repo is a platform for testing the Aruco Detection and landing alogirthm on the drone. This work uses sjtu_drone as a simulation platform.
sjtu_drone is a quadrotor simulation program forked from ['tum_simulator'] (http://wiki.ros.org/tum_simulator) , which is developed with ROS + Gazebo.

# Requirements #
This package is compatible with ROS Melodic version (Ubuntu 18.04).
Please refer the following for the ['installation'](http://wiki.ros.org/Installation/Ubuntu) of ROS on your computer. Prefreable is ROS melodic with ubuntu 18.04 or ROS Noetic with Ubuntu 20.04.

# Download and Compiling this package #
```
$ cd ~/catkin_ws/src
$ git clone https://github.com/Avi241/aruco_detect.git
$ cd ~/catkin_ws
$ catkin_make
```

# Run
The simplest way is calling after you have built the workspace successfully.

```
$ source ~/catkin_ws/devel/setup.bash
$ roslaunch aruco_detect simple.launch
```
# Running with keyboard
In second terminal:

```
$ rosrun aruco_detect drone_keyboard
```
# Steps 

Press Z to takeoff.   Now you can control your drone with keyboars as shown in the Gui


# For Aruco Detection and landing

Go to location ~/catkin_ws/src/aruco_detect/scripts . Open the file ```sample_script.py ``` now you can write your Aruco Detection and landing algorithms here in the main function of this code.\\
<b>Note</b> : If your are using ROS Noetic change the 1st line of the code 

```
#!/usr/bin/env python
```
 to 
 ```
 #!/usr/bin/env python3
```


# To run Aruco Detection and landing program

```
rosrun aruco_detect sample_script.py

```