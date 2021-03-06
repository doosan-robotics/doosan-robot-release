## doosan_robot (kinetic) - 1.0.3-1

The packages in the `doosan_robot` repository were released into the `kinetic` distro by running `/usr/bin/bloom-release doosan_robot --rosdistro kinetic` on `Tue, 07 Jan 2020 05:22:24 -0000`

These packages were released:
- `common`
- `doosan_robot`
- `doosan_robotics`
- `dsr_control`
- `dsr_description`
- `dsr_example_py`
- `dsr_gazebo`
- `dsr_launcher`
- `dsr_msgs`
- `moveit_config_m0609`
- `moveit_config_m0617`
- `moveit_config_m1013`
- `moveit_config_m1509`

Version of package(s) in repository `doosan_robot`:

- upstream repository: https://github.com/doosan-robotics/doosan-robot.git
- release repository: https://github.com/doosan-robotics/doosan-robot-release.git
- rosdistro version: `0.9.6-1`
- old version: `0.9.8-1`
- new version: `1.0.3-1`

Versions of tools used:

- bloom version: `0.9.0`
- catkin_pkg version: `0.4.15`
- rosdep version: `0.15.2`
- rosdistro version: `0.8.0`
- vcstools version: `0.1.42`


## doosan_robot (kinetic) - 0.9.8-1

The packages in the `doosan_robot` repository were released into the `kinetic` distro by running `/usr/bin/bloom-release doosan_robot --rosdistro kinetic` on `Tue, 18 Jun 2019 05:29:02 -0000`

These packages were released:
- `doosan_robot`
- `doosan_robotics`
- `dsr_control`
- `dsr_description`
- `dsr_example_py`
- `dsr_gazebo`
- `dsr_launcher`
- `dsr_msgs`
- `moveit_config_m0609`
- `moveit_config_m0617`
- `moveit_config_m1013`
- `moveit_config_m1509`
- `robotiq_gazebo`
- `serial_node_example`

Version of package(s) in repository `doosan_robot`:

- upstream repository: https://github.com/doosan-robotics/doosan-robot.git
- release repository: https://github.com/doosan-robotics/doosan-robot-release.git
- rosdistro version: `0.9.6-1`
- old version: `0.9.6-1`
- new version: `0.9.8-1`

Versions of tools used:

- bloom version: `0.8.0`
- catkin_pkg version: `0.4.11`
- rosdep version: `0.15.1`
- rosdistro version: `0.7.3`
- vcstools version: `0.1.40`


## doosan_robot (kinetic) - 0.9.6-1

The packages in the `doosan_robot` repository were released into the `kinetic` distro by running `/usr/bin/bloom-release --rosdistro kinetic --track kinetic doosan_robot` on `Mon, 22 Apr 2019 01:56:47 -0000`

These packages were released:
- `doosan_robot`
- `doosan_robotics`
- `dsr_control`
- `dsr_description`
- `dsr_example_cpp`
- `dsr_example_py`
- `dsr_gazebo`
- `dsr_launcher`
- `dsr_msgs`
- `moveit_config_m0609`
- `moveit_config_m0617`
- `moveit_config_m1013`
- `moveit_config_m1509`

Version of package(s) in repository `doosan_robot`:

- upstream repository: https://github.com/doosan-robotics/doosan-robot.git
- release repository: unknown
- rosdistro version: `null`
- old version: `0.9.5-0`
- new version: `0.9.6-1`

Versions of tools used:

- bloom version: `0.8.0`
- catkin_pkg version: `0.4.11`
- rosdep version: `0.15.1`
- rosdistro version: `0.7.3`
- vcstools version: `0.1.40`


## doosan-robot (kinetic) - 0.9.5-0

The packages in the `doosan-robot` repository were released into the `kinetic` distro by running `/usr/bin/bloom-release --rosdistro kinetic --track kinetic doosan-robot` on `Tue, 02 Apr 2019 05:55:08 -0000`

These packages were released:
- `doosan_robot`
- `doosan_robotics`
- `dsr_bringup`
- `dsr_control`
- `dsr_description`
- `dsr_example_cpp`
- `dsr_example_py`
- `dsr_gazebo`
- `dsr_launcher`
- `dsr_msgs`
- `moveit_config_m0609`
- `moveit_config_m0617`
- `moveit_config_m1013`
- `moveit_config_m1509`

Version of package(s) in repository `doosan-robot`:

- upstream repository: https://github.com/doosan-robotics/doosan-robot.git
- release repository: unknown
- rosdistro version: `null`
- old version: `null`
- new version: `0.9.5-0`

Versions of tools used:

- bloom version: `0.7.2`
- catkin_pkg version: `0.4.11`
- rosdep version: `0.15.1`
- rosdistro version: `0.7.2`
- vcstools version: `0.1.40`


# [Doosan robotics](http://www.doosanrobotics.com/kr/)


## Contents
  
  #### [Build](#chapter-2)
  
  #### [Usage](#chapter-3)

# *build* <a id="chapter-2"></a>
    mkdir -p /home/<user_home>/catkin_ws/src
    cd /home/<user_home>/catkin_ws/src
    catkin_init_workspace
    git clone https://github.com/doosan-robotics/doosan-robot
    rosdep install --from-paths doosan-robot --ignore-src --rosdistro kinetic -r -y 
    catkin_make
    source ./devel/setup.bash
#### package list(Internal)
    doosan_robot        ## metapackage
    doosan_robotics     ## metapackage
    dsr_description     ## include URDF, models and description launch files
    dsr_control         ## main-control node(with doosan controller)
    dsr_bringup         ## include hardware information -------- not using
    dsr_example         ## example in ROS envrionment
    dsr_gripper         ## include robotiq_2f_gripper`s description (more gripper will be added)
    dsr_launcher        ## can launch rviz or gazebo simulator with doosan-robot
    dsr_msgs            ## msg and srv files
    moveit_config_m0609 ## moveit for doosan-robot
    moveit_config_m0617 ## moveit for doosan-robot
    moveit_config_m1013 ## moveit for doosan-robot
    moveit_config_m1509 ## moveit for doosan-robot
#### package list(External)
    ros-kinetic-rqt*
    ros-kinetic-moveit*
    ros-kinetic-industrial-core
    ros-kinetic-gazebo-ros-control
    ros-kinetic-joint-state-controller 
    ros-kinetic-effort-controllers 
    ros-kinetic-position-controllers 
    ros-kinetic-ros-controllers
    ros-kinetic-ros-control
    ros-kinetic-serial
    ros-kinetic-lms1xx
    ros-kinetic-interactive-marker-twist-server
    ros-kinetic-twist-mux
    ros-kinetic-imu-tools
    ros-kinetic-controller-manager
    ros-kinetic-robot-localization

# *usage* <a id="chapter-3"></a>
#### dsr_description
```bash
roslaunch dsr_description m0609.launch    
roslaunch dsr_description m1013.launch color:=blue # Change Color
roslaunch dsr_description m1509.launch gripper:=robotiq_2f # insert robotiq gripper
roslaunch dsr_description m0617.launch color:=blue gripper:=robotiq_2f # change color & insert robotiq gripper 필요!
```
#### dsr_moveit_config
> ###### __arguments__
   >color:= ROBOT_COLOR <white  /  blue> defalut = white
   
    roslaunch moveit_config_m0609 m0609.launch
    roslaunch moveit_config_m0617 m0617.launch
    roslaunch moveit_config_m1013 m1013.launch color:=blue
    roslaunch moveit_config_m1509 m1509.launch
    
#### dsr_control _(default model:= m1013, default mode:= virtual)_
> ###### __arguments__                    
>host:= ROBOT_IP defalut = 192,168.137.100   
mode:= OPERATION MODE <virtual  /  real> defalut = virtual  
model:= ROBOT_MODEL <m0609  /  0617/  m1013  /  m1509> defalut = m1013  
color:= ROBOT_COLOR <white  /  blue> defalut = white  
gripper:= USE_GRIPPER <none  /  robotiq_2f> defalut = none  
mobile:= USE_MOBILE <none  /  husky> defalut = none  

#### dsr_control + dsr_moveit_config
    roslaunch dsr_control dsr_moveit.launch
    roslaunch dsr_control dsr_moveit.launch model:=m0609 mode:=virtual
    roslaunch dsr_control dsr_moveit.launch model:=m0617 mode:=virtual
    roslaunch dsr_control dsr_moveit.launch model:=m1013 mode:=virtual
    roslaunch dsr_control dsr_moveit.launch model:=m1509 mode:=virtual
      
#### dsr_launcher
---
> ###### __arguments__
    >host:= ROBOT_IP defalut = 192,168.137.100   
    mode:= OPERATION MODE <virtual  /  real> defalut = virtual  
    model:= ROBOT_MODEL <m0609  /  0617/  m1013  /  m1509> defalut = m1013  
    color:= ROBOT_COLOR <white  /  blue> defalut = white  
    gripper:= USE_GRIPPER <none  /  robotiq_2f> defalut = none  
    mobile:= USE_MOBILE <none  /  husky> defalut = none  

    roslaunch dsr_launcher single_robot_rviz.launch
    roslaunch dsr_launcher single_robot_gazebo.launch
    roslaunch dsr_launcher single_robot_rviz_gazebo.launch
    roslaunch dsr_launcher multi_robot_rviz.launch
    roslaunch dsr_launcher multi_robot_gazebo.launch
    roslaunch dsr_launcher multi_robot_rviz_gazebo.launch
---
#### dsr_example
###### single robot
    <launch>
      single robot in rviz : roslaunch dsr_launcher single_robot_rviz.launch model:=m1013 color:=white
      single robot in gazebo : roslaunch dsr_launcher single_robot_gazebo.launch model:=m1013 color:=blue
      single robot in rviz + gazebo : roslaunch dsr_launcher single_robot_rviz_gazebo.launch model:=m1013 color:=white
    <run application node>
      <cpp>
        basic example : rosrun dsr_example_cpp single_robot_basic dsr01 m1013
        simple example : rosrun dsr_example_cpp single_robot_simple dsr01 m1013
      <py>
        basic example : rosrun dsr_example_py single_robot_basic.py dsr01 m1013
        simple example : rosrun dsr_example_py single_robot_simple.py dsr01 m1013
    <ex>
      roslaunch dsr_launcher single_robot_rviz_gazebo.launch model:=m1013 color:=white
      rosrun dsr_example_cpp single_robot_simple dsr01 m1013

###### multi robot
    <launch>
      multi robot in rviz : roslaunch dsr_launcher multi_robot_rviz.launch
      multi robot in gazebo : roslaunch dsr_launcher multi_robot_gazebo.launch
      multi robot in rviz + gazebo : roslaunch dsr_launcher multi_robot_rviz_gazebo.launch
    <run application node>
      <cpp>
        basic example : rosrun dsr_example_cpp multi_robot_basic
        simple example : rosrun dsr_example_cpp multi_robot_simple
      <py>
        basic example : rosrun dsr_example_py multi_robot_basic.py
        simple example : rosrun dsr_example_py multi_robot_simple.py
      <ex>
        roslaunch dsr_launcher multi_robot_rviz_gazebo.launch
        rosrun dsr_example_cpp multi_robot  

###### robot + mobile
> insert argument mobile:=husky
- single robot on mobile
```bash
roslaunch dsr_launcher rviz_single_robot.launch host:=192.168.137.100 mode:=virtual model:=m1013 color:=blue mobile:=husky
  
<run application node>
  <cpp>
    rosrun dsr_example_cpp single_robot_mobile
  <python>
    rosrun dsr_example_py single_robot_mobile
```
- multi robot on mobile
```bash
roslaunch dsr_launcher rviz_multi_robot.launch host:=192.168.137.100 mode:=virtual model:=m1013 color:=blue mobile:=husky

<run application node>
  <cpp>
    rosrun dsr_example_cpp multi_robot_mobile
  <python>
    rosrun dsr_example_py multi_robot_mobile  
```
###### robot + gripper
> insert argument gripper:=robotiq_2f  
- single robot + gripper
```bash
roslaunch dsr_launcher single_robot_rviz.launch host:=192.168.137.100 mode:=virtual model:=m1013 color:=blue gripper:=robotiq_2f

<run application node>
  <cpp>
    rosrun dsr_example_cpp pick_and_place_simple
  <python>
    rosrun dsr_example_py pick_and_place_simple
```
- Serial Test(Loopback)
```bash
rosrun dsr_example_cpp serial_example_node ttyUSB0 115200
rostopic echo /serial_read
rostopic pub /serial_write std_msgs/String 'data: 100'
```


#### ~~dsr_apps~~
    rosrun dsr_apps_cpp app_watch
    rosrun dsr_apps_cpp app_watch.py
    
#### ~~dsr_test~~
    rosrun dsr_test_cpp dsr_test
    
#### gazebo+rviz+virtual
    roslaunch dsr_example test.launch
    rosrun dsr_test_cpp dsr_test
```bash
  <include file="$(find dsr_gazebo)/launch/dsr_base.launch">
    <arg name="ns" value="dsr01"/> # Robot ID
    <arg name="model" value="m1013"/> # Robot Model
    <arg name="host" value="192.168.137.100"/> # Robot IP
    <arg name="mode" value="virtual"/> # Robot Controller Mode 
    # Position & Posture in Gazebo
    <arg name="x" value="2"/>
    <arg name="y" value="-4"/>
    <arg name="yaw" value="0.7"/>
  </include>
  <include file="$(find dsr_gazebo)/launch/dsr_base.launch">
    <arg name="ns" value="dsr02"/> # Secondary Robot ID
    <arg name="model" value="m1013"/> # Secondary Robot Model
    <arg name="host" value="192.168.137.102"/> # Secondary Robot IP
    <arg name="mode" value="virtual"/> # Secondary Robot Controller Mode
    # Secondary Position & Posture in Gazebo
    <arg name="x" value="2"/>
    <arg name="y" value="-4"/>
    <arg name="yaw" value="0.7"/>
  </include>
```  

#### Run multi-robot by command line
```bash
roslaunch dsr_launcher test.launch
rostopic pub /dsr01m1013/joint_position_controller/command std_msgs/Float64MultiArray "layout:
  dim:
  - label: ''
    size: 0
    stride: 0
    data_offset: 0
data: [10, 10, 40, 10, 60, 10]"
```
#### Service Call
```bash
rosservice call /dsr/set_joint_move "jointAngle: [0.0, 0.0, 0.0, 0.0, 0.0, 0.0]
jointVelocity: [50.0, 0.0, 0.0, 0.0, 0.0, 0.0]
jointAcceleration: [50.0, 0.0, 0.0, 0.0, 0.0, 0.0]
radius: 0.0"
```

#### Run Mobile Robot 
+ Install external package for kinetic
```python  
sudo apt install ros-kinetic-interactive-markers
sudo apt install ros-kinetic-interactive-marker-twist-server
sudo apt install ros-kinetic-twist-mux ros-kinetic-twist-mux-msgs ros-kinetic-robot-localization
```
+ Install external package for melodic
```python      
sudo apt install ros-melodic-interactive-markers
sudo apt install ros-melodic-twist-mux ros-melodic-twist-mux-msgs ros-melodic-robot-localization      
#sudo apt install ros-melodic-interactive-marker-twist-server (not-exist) need form src install
#ros-melodic-interactive-marker-twist-server for source install
cd ~/catkin_ws/src
git clone https://github.com/ros-visualization/interactive_marker_twist_server.git
rosdep install --from-paths ~/catkin_ws/src --ignore-src
cd ~/catkin_ws
catkin_make
source ~/catkin_ws/devel/setup.bash
```

```bash
#roslaunch dsr_launcher multi_gazebo.launch mobile:=true
roslaunch dsr_launcher mobile_m1013.launch
or
roslaunch dsr_launcher mobile_robot.launch model:=m1013 color:=white
rosrun dsr_example_cpp m1013_on_mobile
```

# diagnostic

# etc
