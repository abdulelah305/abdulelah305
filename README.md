# Installing ROS on Ubuntu 20.04 this will describe step by step the proccess 


### Table of contents 

* [Installation](#installation)
* [ROS](#ros)
* [ROS Melodic](#ros-melodic)
 * [Catkin Workspace](#catkin-workspace)
* [Testing](#testing)
* [Concluion](#concluion)
 

## Installation


### ROS

Install the `ros-melodic-ros-base` package on your  following these directions:

* ROS Melodic - [ROS Install Instructions](http://wiki.ros.org/melodic/Installation/Ubuntu)


Depending on which version of ROS you're using, install some additional dependencies and create a workspace:

#### ROS Melodic

A fast way to install ROS is to clone the following repo
```bash
$ git clone https://github.com/JetsonHacksNano/installROS
```
then runing the InstallROS.sh file and giving it the name of the package as follows :
`$ ./installROS.sh -p ros-melodic-desktop -p ros-
melodic-rgbd-launch`
here we downloaded the desktop melodic version.



#### Catkin Workspace 

then we need to make a Catkin Workspace and as we can see in this repo the file 
**setupCatkinWorkspace.sh** is built to help in creating the catkin workspace.
You can edit this file to add the ROS packages for your application.
Usage:
`$ ./setupCatkinWorkspace.sh 
[_optionalWorkspaceName_]`
where _optionalWorkspaceName_ is the name and path of the workspace to be used.
The default workspace name is `~/catkin_ws`.




## Testing

Before proceeding, if you're using ROS Melodic make sure that 'roscore' is running first:
'''bash
$ roscore
'''
![code](https://user-images.githubusercontent.com/110297601/181924991-d51021e0-f79f-447a-991d-c55a264109d1.jpg)

## Concluion 

there are few ways to install and set up ROS on Jetson Nano which usually is a straight fowrward process. 
I chose to do this task using this method since it simplifies the process and prevent possiople errors.
