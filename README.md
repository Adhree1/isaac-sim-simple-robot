# isaac-sim-simple-robot
Physics-based differential drive robot simulation using NVIDIA Isaac Sim and ROS 2 with LiDAR and RViz visualization.

 
🚗 Simple Mobile Robot Simulation
NVIDIA Isaac Sim 4.x · ROS 2 Jazzy · RViz
📌 Overview

This project demonstrates the development of a physics-based differential-drive mobile robot using NVIDIA Isaac Sim with full ROS 2 Jazzy integration.
The project focuses on realistic robot modeling, physics configuration, sensor integration, and real-time data streaming to ROS 2 for visualization and future autonomy tasks.

This repository serves as a foundational robotics simulation portfolio project, showcasing industry-relevant skills in simulation, control, and perception.

🧠 What This Project Demonstrates

Robotics simulation using NVIDIA Isaac Sim

Physics-based robot modeling

Differential drive control

Sensor integration (RGB Camera & 2D LiDAR)

ROS 2 Jazzy communication

Real-time visualization in RViz

🛠️ Technologies Used

NVIDIA Isaac Sim 4.x

ROS 2 Jazzy

PhysX Physics Engine

RViz

OmniGraph

USD (Universal Scene Description)

🤖 Robot Description

The robot is a rear-wheel-drive differential mobile robot consisting of:

A rigid chassis

Four wheels (rear wheels driven, front wheels passive)

Revolute joints for wheel rotation

Fixed joints for sensor mounting

Physics-based collision and rigid body configuration

⚙️ Physics & Control

Configured Rigid Bodies, Collision Shapes, and Joints

Used Angular Drives on rear wheels for velocity control

Tuned damping for stable and precise wheel motion

Implemented differential drive logic using OmniGraph and ROS 2

📡 Sensor Integration

The robot is equipped with:

RGB Camera (front-facing)

2D Rotating LiDAR (PhysX LiDAR)

Sensors are mounted on a dedicated sensor frame and physically attached to the robot body using Fixed Joints to ensure correct motion and TF consistency.

🔁 ROS 2 Integration

Enabled ROS 2 Bridge

Published:

/scan_lidar (LaserScan)

/tf and /tf_static

Visualized sensor data and transforms in RViz

Verified real-time streaming and correct frame alignment

📊 Visualization

LiDAR data visualized as LaserScan in RViz

TF tree validated for correct frame relationships

Sensor debug visualization enabled inside Isaac Sim

🎯 Learning Outcomes

Through this project, I gained hands-on experience in:

Navigating and using the Isaac Sim interface

Building robot models using USD Prims

Configuring realistic physics interactions

Understanding joints, damping, and constraints

Attaching sensors correctly in a physics simulation

Streaming simulation data to ROS 2 Jazzy

Debugging TF trees and sensor frames

Visualizing robotics data using RViz

🚀 Future Work

Planned extensions include:

Odometry publishing

SLAM using slam_toolbox

Navigation using Nav2

/cmd_vel velocity control

Multi-sensor fusion (camera + LiDAR)

Autonomous navigation experiments

📸 Demo (Coming Soon)

Isaac Sim simulation video

RViz LiDAR & TF screenshots

SLAM visualization

👤 Author

Adhree Pradeep
Robotics & Simulation
Focused on ROS 2, Isaac Sim, and autonomous systems

⭐ Portfolio Note

This project demonstrates practical, simulation-first robotics skills aligned with real-world mobile robot development workflows.
