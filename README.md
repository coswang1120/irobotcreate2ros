irobotcreate2ros
===
Ros node for iRobot Create 2.

Prerequisites
---
* [ros serial](http://wiki.ros.org/rosserial)
* [ros joy](http://wiki.ros.org/joy)

Compiling
---
Just clone the repository in the src folder of a catkin workspace. Then run catkin_make.

Usage
---
---
```
rosrun irobotcreate2 irobotcreate2
```
to run the basic software and have access to the following topics:

- /battery
- /bumper
- /buttons
- /cliff
- /cmd_vel
- /digit_leds
- /ir_bumper
- /ir_character
- /leds
- /mode
- /odom
- /play_song
- /rosout
- /rosout_agg
- /song
- /tf
- /wheel_drop

you can read sensors (/battery, /buttons, /bumper, ...) and send commands (/cmd_vel, ...).

---
```
rosrun irobotcreate2 irobot_joy.launch
```
to run both the basic software and ros joy to move the robot with a controller.