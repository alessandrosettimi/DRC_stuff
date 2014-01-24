Prepare a vanilla-ubuntu 13.04 for the DRC stuff:
=========

- install ros following: http://wiki.ros.org/hydro/Installation/Ubuntu

- install catkin following: http://wiki.ros.org/catkin

- create a catkin workspace following: http://wiki.ros.org/catkin/Tutorials/create_a_workspace

- clone the yarp repository: https://github.com/robotology/yarp

- install yarp following: http://wiki.icub.org/wiki/Linux:Installation_from_sources#Getting_the_YARP_and_iCub_sources
                     and: http://wiki.icub.org/wiki/Linux:Installation_from_binaries
  -> use the CREATE_SHARED_LIBRARY option in the ccmake!!

- related packages: 
```
- https://github.com/EnricoMingo/iit-coman-ros-pkg
- https://github.com/robotology/gazebo_yarp_plugins
- https://github.com/valeriovarricchio/DRC_catkin -> dependencies: ros-hydro-joy*, ros-hydro-openni2-*
```

You can put these lines in your .bashrc if you want:
```
export YARP_ROOT=/home/user/projects/yarp
source /opt/ros/hydro/setup.bash
source /home/user/catkin_ws/devel/setup.bash
export ROS_PACKAGE_PATH=${ROS_PACKAGE_PATH}:/home/user/..../iit-coman-ros-pkg
```
