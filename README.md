# SmartMethod-1stTask-Ros-OS
First task in robotics and AI path(install Ros OS on Ubuntu 20.4)


## Table of Contents
* [Technologies Used](#technologies-used)
* [Setup](#setup)
* [Screenshots](#Screenshots)
* [Acknowledgements](#acknowledgements)




## Technologies Used
- Ubuntu - version 20.04.4
- VirtualBox - version 6.1.34
- ROS Neotic



## Setup
First of all you have to install VirtualBox in this link https://www.virtualbox.org/wiki/Downloads
There is two type of ROS OS (Melodic & Neotic).

Ubuntu Instalation :

To can install ROS Melodic OS you have to download one of this Ubuntu versions:
Ubuntu Artful (17.10):http://old-releases.ubuntu.com/releases/17.10/
Ubuntu Bionic (18.04): https://releases.ubuntu.com/18.04/.


  OR
                                  
install Ubuntu Focal Fossa (20.04) for ROS Neotic: https://releases.ubuntu.com/20.04/

This tutorial for Install ROS Neotic.

1- Setup your VB and install Ubuntu OS in it by follow this tutorial :https://www.geeksforgeeks.org/how-to-install-ubuntu-on-virtualbox/
2-Install ROS OS:
   2.1 Setup your sources.list:
       Setup your computer to accept software from packages.ros.org.
       
        `sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list`
        
        
   2.2 Set up your keys:
   
        `curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -`

   ** if curl not exist  run `sudo apt install curl ` **
   
   outbut should be "ok".
         
         
   2.3  make sure your Debian package index is up-to-date:
   
          `sudo apt update`
        
        
   2.4 Install ROS 
       Desktop-Full Install Everything in Desktop plus 2D/3D simulators and 2D/3D perception packages
       
        `sudo apt install ros-noetic-desktop-full`
        
        
   2.5 Environment setup
        You must source this script in every bash terminal you use ROS in.
        
         `source /opt/ros/noetic/setup.bash`
         `echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc
          source ~/.bashrc`
          
Now ROS OS are installed in your device and ready to use.



## Screenshots
1- Setup sources.list && key

![1 Setup sources.list && key](./ScreenShots/First.png)
2- Instlattion

![2 Instlattion](./ScreenShots/installation.png)
3- Environment setup

![3 Environment setup](./ScreenShots/End.png)
4-logo of ROS OS

![4 logo of ROS OS](./ScreenShots/logo.png)
5-ROS Interface

![5 ROS Interface](./ScreenShots/interface.png)

<!-- If you have screenshots you'd like to share, include them here. -->




## Acknowledgements
credit:

- This Tutorial was based on ROS Documntation.


