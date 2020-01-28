# Exploring-my-Blender-world-with-Turtlebot-in-gazebo-with-ros-melodic

This repo contains my ros workspace. It has the packages for turtlebot and turtlebot_simulator for gazebo this is for ROS melodic compatible with Ubuntu 18.04
<br>
How to do it for yourself : <br>
- Install ROS melodic on Ubuntu 18.04, Open terminal<br>
this is just the tip of the iceberg, you can see <a href="http://wiki.ros.org/melodic/Installation/Ubuntu">Official instalation Instruction </a>
<code>
sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
</code><p><br>
<code>
sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
</code><p><br>

<code>
sudo apt update
sudo apt install ros-melodic-desktop-full
</code><br><p>

<code>
sudo rosdep init
rosdep update
</code><br><p>

<code>
echo "source /opt/ros/melodic/setup.bash" >> ~/.bashrc
source ~/.bashrc
</code><br><p>

<code>
sudo apt install python-rosinstall python-rosinstall-generator python-wstool build-essential
</code><br><p>

- make a work space<br>
<code>
mkdir ~/Anurag_turtlebot_ws
</code><br>
<code>
cd ~/Anurag_turtlebot_ws
</code><br>
<code>
mkdir src; cd src 
</code><br>
<code>
git clone https://github.com/AnuragSahu/Exploring-my-Blender-world-with-Turtlebot-in-gazebo-with-ros-melodic.git
</code><br>
<code>
cd .. 
</code><br>
<code>
catkin_make 
</code><br>

- Take a break You must have encountered a lot of errors until now and you deserve a break, but if you are stuck at some point please make a issue I might be able to help you.
- Moment of truth! Run the code
<code>
source ~/Anurag_turtlebot_ws/devel/setup.bash
</code><p><br>
<code>
roslaunch turtlebot_gazebo turtlebot_world.launch
</code>
