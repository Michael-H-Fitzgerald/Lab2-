# Lab2- 
**Navvis Description robot for lab two** <br />
***Setup Envirnment*** <br />
Install ros melodic at http://wiki.ros.org/melodic/Installation/Ubuntu <br />
Once the correct version of ROS is installed open the a terminal on your Ubuntu laptop <br />
Create a directory for your ROS workspace (named something similar to Navvis or lab2) <br />
Then run this command <br />
```source /ros/melodic/setup.bash``` <br />
Then go into your workspace <br />
```cd lab2``` <br />
Then create a source directory <br />
```mkdir src``` <br />
Then create run the catkin_make command <br />
```catkin_make``` <br />
After create the dev env <br />
```source devel/setup.bash``` <br />
Finally run these last two commands <br />
```cd src```
```catkin_create_pkg navvis_description rviz urdf xacro sensor_msgs geometry_msg``` <br />
```cd navvis_description``` <br />
After clone the repository in the navvis_Description <br />
```git clone https://github.com/Michael-H-Fitzgerald/Lab2``` <br />
Finally make the catkin file again <br />
```cd ../../``` <br />
```catkin_make clean``` <br />
***Run Navvis Robot*** <br />
***run with no gui*** <br />
```roslaunch navvis_description navvis_launch &``` <br />
***run with joint state publisher** <br />
```roslaunch navvis_description navvis_launch use_jsp_gui:=false &``` <br />
***run with and without the xacro*** <br />
```use_xacro:=true or use_xacro:=false``` <br />
