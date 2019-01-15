
# Turtlebot3 Autorace

#### How to run
1. Add following lines in .bashrc

```
export GAZEBO_MODE=true
export AUTO_IN_CALIB=action
export AUTO_EX_CALIB=action
export AUTO_DT_CALIB=action
export TURTLEBOT3_MODEL=burger
```


2. To run enter following commands in different terminals

> roslaunch turtlebot3_gazebo turtlebot3_autorace.launch

> roslaunch turtlebot3_gazebo turtlebot3_autorace_mission.launch

> roslaunch turtlebot3_autorace_camera turtlebot3_autorace_intrinsic_camera_calibration.launch

> roslaunch turtlebot3_autorace_core turtlebot3_autorace_core.launch

> rostopic pub -1 /core/decided_mode std_msgs/UInt8 "data: 2"
