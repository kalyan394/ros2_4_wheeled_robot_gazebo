# ROS2 mobile robot in ignition gazebo
- This code is for launching the gazebo launch files in Ignition gazebo by having urdf files and also Rviz files.

### Things done
- Workspace 
- Creation of Robot through URDF in XML
- Launch files
- RVIZ2 and ignition gazebo

## Commands I used in Ros2
1. Before start we need to source the terminal by using following command
  -   source /opt/ros/foxy/setup.bash
2. Navigate to work space and enter foolowing command
   -  . install/setup.bash
3. Next we need to compile all the packages by using
   -  colcon build
4. To launch gazebo file
    - ros2 launch rover 2_gazebo_spawn.launch.py
5.  To launch rviz file
    - ros2 launch rover 1_Rviz.launch.py
 6. To move the in gazebo 
    - ros2 run teleop_twist_keyboard teleop_twist_keyboard 
    
7.Everything is succesful in gazebo but in Ignition gazebo its not working

8. To select only one package use following command
      - colcon build --symlink-install --packages-select rover(package_name).
9. For cloning use below one by navigating to the workspace
    - git clone https://github.com/kalyan394/ros2_mobile_robot.git
    
## Ignition gazebo version :

     Ignition Gazebo, version 3.13.0
Copyright (C) 2018 Open Source Robotics Foundation.
Released under the Apache 2.0 License.
                                                          

## System Requirements
- Ubuntu 20.04
- ROS2 Foxy
- Visual Studio Code

