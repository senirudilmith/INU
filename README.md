# Quadruped Robot: Accessible Design for Education and Research

This repository provides the **design, development, and control** resources for a quadruped robot. Built with cost-efficiency and accessibility in mind, this project allows users to explore advanced robotics concepts, such as inverse kinematics, multi-degree-of-freedom control, and natural locomotion patterns.

---


<div>
  <img src="https://github.com/user-attachments/assets/2a7660c4-2bd7-4225-9094-e3b8aaed3a98" alt="Front View of INU" style="display: block; margin-bottom: 100px; width: 8000px;">
  <div align="center"><em>Front View of INU</em></div>
</div>

<div style="margin-top: 20px;">
  <img src="https://github.com/user-attachments/assets/5de48070-1751-4b7a-a934-e79c7125de1f" alt="Top View of INU" style="display: block; margin-bottom: 100px; width: 1000px;">
  <div align="center"><em>Top View of INU</em></div>
</div>



## Table of Contents
1. [Project Overview](#project-overview)
2. [Key Features](#key-features)
3. [System Requirements](#system-requirements)
4. [Hardware Architecture](#hardware-architecture)
5. [Software Architecture](#software-architecture)
6. [Control System](#control-system)
7. [Design and 3D Models](#design-and-3d-models)
8. [Performance and Limitations](#performance-and-limitations)
9. [Future Enhancements](#future-enhancements)
10. [Contributing](#contributing)

---

## Project Overview

### Objectives
1. Develop a **low-cost quadruped robot** for educational and research purposes.
2. Implement robotics techniques such as inverse kinematics and synchronized leg movement.
3. Provide a modular, customizable platform for experimentation and learning.

### Applications
- Robotics education and research.
- Exploration of hazardous or uneven terrains.
- Human-robot interaction studies.

---

## Key Features

- **Cost-Efficient Design**: Built under LKR 25,000 (~$75 USD).
- **Arduino-Based Control System**: Simplifies control and programming.
- **Inverse Kinematics**: Ensures stable, synchronized locomotion.
- **3D-Printed Components**: Easy-to-reproduce parts using standard 3D printers.
- **Interactive OLED Display**: Provides real-time feedback and status updates.

---

## System Requirements

### Hardware
- **Arduino Uno** (Microcontroller)
- **MG90S Micro Servo Motors** (12 units for locomotion)
- **Capacitive Touch Sensor (TTP223)**
- **Arduino Sensor Shield**
- **0.96-inch OLED Display**

### Software
- **Arduino IDE** (1.8.x or later) for programming.
- **Blender** (For 3D modeling and design).
- **SolidWorks** (For structural analysis and simulations).

---

## Hardware Architecture

### Component List
| **Component**                      | **Description**                            | **Estimated Cost (LKR)** |
|------------------------------------|--------------------------------------------|--------------------------|
| Arduino Uno                        | Main microcontroller for control logic      | 1200                    |
| MG90S Micro Servo Motors (12 units)| Actuators for robotic leg movements         | 8000                    |
| Capacitive Touch Sensor (TTP223)   | Detects touch input for starting/stopping   | 1000                    |
| Arduino Sensor Shield              | Simplifies sensor and motor connections     | 500                     |
| 0.96-inch OLED Display             | Displays system diagnostics and status      | 1000                    |
| 3D-Printed Parts                   | Robot chassis and legs                      | 10000                   |
| **Total Estimated Cost**           |                                            | **25000**               |

---

## Software Architecture

### Key Components
1. **Control Logic**:
   - Implemented in **C++** using the Arduino IDE.
   - Supports inverse kinematics and gait cycle generation.

2. **Locomotion Patterns**:
   - Predefined walking and turning sequences.
   - Adjustable via servo angles.

3. **Real-Time Feedback**:
   - Displays diagnostic data on a 0.96-inch OLED.

For complete code, visit the [Software Directory](Software/Arduino/main.ino).

---

## Control System

The control system leverages **inverse kinematics (IK)** to calculate precise servo angles for stable leg movements. It translates desired positions in Euclidean space into servo commands, ensuring coordinated and efficient locomotion.

### Key Workflow
1. Define target positions for each leg in the coordinate space.
2. Compute joint angles using inverse kinematic equations.
3. Send calculated commands to the servos for execution.

For a detailed implementation, see the [main.ino file](Software/Arduino/main.ino).

---

## Design and 3D Models

### Workflow
- **Blender**: Designed all structural components with precision.
- **SolidWorks**: Simulated and validated structural integrity, motion, and thermal performance.
- **STL Files**: Printable models available in the [Models/STL](Models/STL/) directory.

---

## Performance and Limitations

### Achievements
- Successfully implemented stable walking and turning gaits.
- Demonstrated functionality on both flat and uneven terrains.
- Modular design supports rapid assembly and part replacement.

### Limitations
- No integrated obstacle detection sensors.
- Battery runtime limited to ~1 hour of continuous operation.
- Servo motors produce noticeable noise during operation.

---

## Future Enhancements

1. **Sensor Integration**:
   - Add ultrasonic or LiDAR sensors for obstacle avoidance.
2. **Battery Optimization**:
   - Extend runtime with high-capacity rechargeable batteries.
3. **Enhanced Control**:
   - Introduce brushless motors for smoother and quieter operation.
4. **AI Integration**:
   - Enable path-planning and autonomous navigation capabilities.

---

## Contributing

We welcome contributions to this project! Follow these steps to contribute:
1. Fork the repository.
2. Create a feature branch (`git checkout -b feature-name`).
3. Commit your changes (`git commit -m "Description of changes"`).
4. Push to the branch (`git push origin feature-name`).
5. Submit a pull request.

---


