# MobRob_ROS_gazebo
ROS-Package: **mobrob_gazebo** package for MobRob (gazebo simulator)

![alt text](https://techniccontroller.de/wp-content/uploads/gazebo.jpg "Simulated robot model of MobRob in Gazebo")

More information on my website: https://techniccontroller.de/mobrob-ros-software-architecture/

## Instructions

Run following command to start gazebo with MobRob model:

```
roslaunch mobrob_gazebo myrobot_world.launch
```


Control the robot via **teleop_twist_keyboard**

Install:
```commandline
sudo apt-get install ros-noetic-teleop-twist-keyboard
```

Run:
```commandline
rosrun teleop_twist_keyboard teleop_twist_keyboard.py
```

Control:
```commandline
Reading from the keyboard  and Publishing to Twist!
---------------------------
Moving around:
   u    i    o
   j    k    l
   m    ,    .

For Holonomic mode (strafing), hold down the shift key:
---------------------------
   U    I    O
   J    K    L
   M    <    >

t : up (+z)
b : down (-z)

anything else : stop

q/z : increase/decrease max speeds by 10%
w/x : increase/decrease only linear speed by 10%
e/c : increase/decrease only angular speed by 10%

CTRL-C to quit
```

