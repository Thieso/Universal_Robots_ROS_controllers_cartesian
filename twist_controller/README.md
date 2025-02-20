# Twist Controller

A Cartesian ROS-controller for commanding target twists to a robot.

This controller makes use of a `TwistCommandInterface` to set a user specified
twist message as reference for robot control.

## Controller .yaml
A possible configuration looks like this:

```yaml
twist_controller:
   type:         ros_controllers_cartesianlers/TwistController

   # The controller uses this identifier to get the according command handle
   # from the hardware interface.
   frame_id:     "endpoint_to_control"

   joints:
   - joint1
   - joint2
   - joint3
   - joint4
   - joint5
   - joint6
```

## Acknowledgement
Developed in collaboration between:

[<img height="60" alt="Universal Robots A/S" src="../ros_control_cartesian/doc/resources/ur_logo.jpg">](https://www.universal-robots.com/) &nbsp; and &nbsp;
[<img height="60" alt="FZI Research Center for Information Technology" src="../ros_control_cartesian/doc/resources/fzi_logo.png">](https://www.fzi.de).

***
<!--
    ROSIN acknowledgement from the ROSIN press kit
    @ https://github.com/rosin-project/press_kit
-->

<a href="http://rosin-project.eu">
  <img src="http://rosin-project.eu/wp-content/uploads/rosin_ack_logo_wide.png"
       alt="rosin_logo" height="60" >
</a>

Supported by ROSIN - ROS-Industrial Quality-Assured Robot Software Components.
More information: <a href="http://rosin-project.eu">rosin-project.eu</a>

<img src="http://rosin-project.eu/wp-content/uploads/rosin_eu_flag.jpg"
     alt="eu_flag" height="45" align="left" >

This project has received funding from the European Union’s Horizon 2020
research and innovation programme under grant agreement no. 732287.
