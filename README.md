# Autonomous Driving using Machine Learning (Unity + Python)

#  Overview

This project implements a real-time autonomous vehicle navigation system using Unity simulation and a custom machine learning pipeline.

The system learns driving behavior from human input using **behavioral cloning** and performs real-time inference to drive autonomously.


## &#x20;System Architecture

* **Unity (C#)** → Simulation, vehicle physics, sensors
* **Python (PyTorch)** → Neural network training & inference
* **TCP Communication** → Real-time data exchange


## &#x20;Features

* Real-time ML training
* Behavioral cloning (learns from human driving)
* 3 Driving Modes:

  * Manual
  * Scripted (Waypoint-based)
  * ML Autonomous Driving
* 9 Raycast sensors (LIDAR-like)
* Waypoint navigation system


## &#x20;System Flow

Sense → Send → Train → Predict → Act


## &#x20;ML Details

* Model: Feedforward Neural Network
* Input: 20 features
* Output: Steering + Acceleration
* Loss: MSE
* Optimizer: Adam


## &#x20;Results

* 6000+ frames collected
* Loss reduced from ~0.088 → ~0.01
* Stable autonomous driving in simulation


## &#x20;Tech Stack

* Unity 2021 (C#)
* Python 3.9
* PyTorch
* NumPy, Pandas
* TCP Socket Programming


##  How to Run

### 1. Start Python Server

```bash
python realtime_server.py
```

### 2. Run Unity Project

* Open Unity
* Press Play
* Press `P` to connect
* Press `M` for ML driving

##  Future Scope

* Real-world implementation
* Camera-based vision (CNN)
* Reinforcement learning
* 
##  Project Structure

- Assets/ → Unity project files  
- ProjectSettings/ → Unity configuration  
- realtime_server.py → ML training server  
- README.md → Documentation  


## Project Highlights

- Built a real-time ML pipeline integrating Unity and Python via TCP
- Implemented behavioral cloning for autonomous driving
- Designed sensor-based perception using raycasting (LIDAR-like)
- Achieved significant loss reduction (~0.088 → ~0.01)
- Enabled continuous learning across sessions using replay buffer

## 👨‍💻 Author

Janmejay Rashinkar
B.E. Electronics & Telecommunication Engineering Honors AIML 
