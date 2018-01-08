# Velodyne-in-ROS
Install Velodyne in ROS environment

https://github.com/ros-drivers/velodyne

## Install Velodyne Driver
```
$ sudo apt-get update
$ sudo apt-get upgrade

$ mkdir -p ~/catkin_ws/src
$ cd ~/catkin_ws/src
$ git clone https://github.com/ros-drivers/velodyne.git
```
Install dependences into rosdistro kinetic

```
$ cd ..
$ rosdep install --from-paths src --ignore-src --rosdistro kinetic -y
```

Make and source
```
$ catkin_make
$ source devel/setup.bash
```

## Test the Velodyne pointcloud
I am using the Udacity Challenge 3 dataset. 
https://medium.com/udacity/challenge-3-image-based-localization-5d9cadcff9e7.
