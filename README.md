# Isaac Sim Simple Robot

Physics-based differential drive mobile robot simulation using NVIDIA Isaac Sim and ROS 2 Jazzy with LiDAR visualization in RViz.

---

## Overview

This project demonstrates the development of a **physics-based differential-drive mobile robot** using **NVIDIA Isaac Sim 4.x** with full **ROS 2 Jazzy** integration.  
The focus of this work is on realistic robot modeling, physics configuration, sensor integration, and real-time data streaming to ROS 2 for visualization and future autonomy tasks.

This repository serves as a **foundational robotics simulation portfolio project**, showcasing practical skills in simulation, control, and perception.

---

## Project Objectives

The primary objectives of this project are to:

- Build a mobile robot model using USD primitives in Isaac Sim  
- Configure realistic physics interactions using the PhysX engine  
- Implement differential drive control using joint-based actuation  
- Integrate perception sensors including an RGB camera and 2D LiDAR  
- Stream sensor and transform data to ROS 2 Jazzy  
- Visualize robot state, sensors, and TF frames in RViz  

---

## Robot Description

The simulated robot is a **rear-wheel-drive differential mobile robot** consisting of:

- A rigid chassis body
- Four wheels (rear wheels driven, front wheels passive)
- Revolute joints for wheel rotation
- Fixed joints for rigid sensor mounting
- Physics-based collision and rigid body properties

The robot is designed to reflect common real-world mobile robot architectures used in research and industry.

---

## Physics and Control Configuration

- Rigid bodies and collision meshes configured for all physical components
- Revolute joints used for wheel actuation
- Angular drives applied to rear wheel joints for velocity control
- Damping tuned to ensure stable and smooth motion
- Differential drive behavior implemented via OmniGraph and ROS 2 interfaces

---

## Sensor Integration

The robot is equipped with the following sensors:

- **RGB Camera** (front-facing)
- **2D Rotating LiDAR (PhysX LiDAR)**

Sensors are mounted on a dedicated sensor frame and physically attached to the robot chassis using **fixed joints**, ensuring correct motion coupling and transform consistency.

---

## ROS 2 Integration

This project integrates Isaac Sim with **ROS 2 Jazzy** using the ROS 2 Bridge:

- LiDAR data published as `sensor_msgs/LaserScan`
- Transform data published on `/tf` and `/tf_static`
- Real-time data streaming validated during simulation
- Visualization and debugging performed using RViz

---

## Visualization

- LiDAR scans visualized as LaserScan data in RViz
- TF tree validated for correct frame relationships
- Sensor debug visualization enabled within Isaac Sim

---

## Technologies Used

- NVIDIA Isaac Sim 4.x  
- ROS 2 Jazzy  
- PhysX Physics Engine  
- OmniGraph  
- RViz  
- USD (Universal Scene Description)

---

## Learning Outcomes

Through this project, the following competencies were developed:

- Proficient navigation of the Isaac Sim interface and USD stage hierarchy
- Understanding of physics-based robot modeling and joint configuration
- Practical experience with differential drive control
- Correct attachment and configuration of sensors in a physics simulation
- ROS 2 data streaming and TF debugging
- Visualization of robotic perception data in RViz

---

## Future Work

Potential extensions to this project include:

- Wheel odometry publishing
- SLAM integration using `slam_toolbox`
- Autonomous navigation using Nav2
- Velocity control via `/cmd_vel`
- Multi-sensor fusion
- Closed-loop navigation experiments

---

## Author

**Adhree Pradeep**  
Robotics and Simulation  
Focus areas: ROS 2, Isaac Sim, Mobile Robotics, Autonomous Systems
