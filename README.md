# Lab2-
**Navvis Description robot for lab two**
***Setup Envirnment***
Install ros melodic at http://wiki.ros.org/melodic/Installation/Ubuntu
Once the correct version of ROS is installed open the a terminal on your Ubuntu laptop
Create a directory for your ROS workspace (named something similar to Navvis or lab2)
Then run this command
```source /ros/melodic/setup.bash```
Then go into your workspace
```cd lab2```
Then create a source directory 
```mkdir src```
Then create run the catkin_make command
```catkin_make```
After create the dev env  
```source devel/setup.bash
Finally run these last two commands 
```cd src```
```catkin_create_pkg navvis_description rviz urdf xacro sensor_msgs geometry_msg```
```cd navvis_description```
After clone the repository in the navvis_Description 
```git clone https://github.com/Michael-H-Fitzgerald/Lab2```
Finally make the catkin file again 
```cd ../../```
```catkin_make clean```
***Run Navvis Robot***
***run with no gui***
```roslaunch navvis_description navvis_launch &```
***run with joint state publisher**
```roslaunch navvis_description navvis_launch use_jsp_gui:=false &```
***run with and without the xacro***
```use_xacro:=true or use_xacro:=false```
