---
layout: page
title: ROS2swarm
description: A ROS 2 package
img: assets/img/ROS2swarm_TB.jpg
importance: 2
category: work
---

ROS2swarm is a ROS 2 package intended to simplify and promote the use of ROS 2 in swarm robotics research, industry, and education. 
It is an easy-to-extend framework for and library of swarm behaviors.


<div class="row justify-content-sm-center">
    <div class="col-sm-4 mt-3 mt-md-0">
{% include figure.html path="assets/img/ROS2swarm_TB.jpg" title="TurtleBot3 Waffle Pis in an arena." class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
{% include figure.html path="assets/img/ROS2swarm_TB.jpg" title="TurtleBot3 Waffle Pis in an arena." class="img-fluid rounded z-depth-1" %}
    </div>
</div>
A swarm of seven TurtleBot 3 Waffle Pis in an arena bounded by walls. 

ROS2swarm currently provides six movement patterns for robot motion and two voting patterns for collective decision-making. We distinguish between basic patterns that implement primitive swarm behaviors and combined patterns that implement more complex behaviors. Parameter files allow the adjustment of patterns for different robot platforms and scenarios. In addition, we included a hardware protection layer to prevent hardware damage.

The package is available for Dashing and Foxy since our main development platform is the TurtleBot3 Waffle Pi. Furthermore, we provide out-of-the-box support for the TurtleBot3 Burger and the Jackal UGV (using the ros1_bridge 5 package). We also provide simulations in Gazebo for all three platforms to simplify development. New platforms that provide distance measurements in a LaserScan message and are controlled by linear velocities along the x-axis and rotational velocities around the z-axis can easily be added.

Currently, we are working on integrating support for robots with less sophisticated sensor setups, such as the Thymio II, enabling local communication, and adding more swarm behaviors.

The code for ROS2swarm is available on <a href="https://github.com/ROS2swarm">Github</a>.
