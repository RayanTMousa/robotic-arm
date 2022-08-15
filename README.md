# robotic-arm
You have to create catkin workspace folder. To do that :
$ mkdir -p ~/catkin_ws/src
$ cd ~/catkin_ws/
$ catkin_make

 Download dependencies  
- run this command inside the worspace 
$ rosdep install --from-paths src --ignore-src -r -y
-then install
$ sudo apt-get install ros-melodic-moveit
$ sudo apt-get install ros-melodic-joint-state-publisher ros-melodic-joint-state-publisher-gui
$ sudo apt-get install ros-melodic-gazebo-ros-control joint-state-publisher
$ sudo apt-get install ros-melodic-ros-controllers ros-melodic-ros-control

- Download Arm Packages from https://github.com/smart-methods/arduino_robot_arm
-  Move the downloaded folder ( arduino robot arm ) to src which is located inside the catkin_ws ( workspace)
- open terminal from inside the folder
- write: cd ..
catkin_make
sudo nano ~/.bashrc
- at the end of the page write 
source /home/me/catkin_ws/devel/setup.bash
then ctrl + o then ctrl + x
- write these commands in terminal
source ~/.bashrc
roslaunch robot_pkg check_motors.launch

 the program will be downloaded and opened ( Rivz ) and launched.
