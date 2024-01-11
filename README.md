
# TurtleBot3 Burger Teleoperation with Niryo Ned

## Project Overview
This project enables the teleoperation of a TurtleBot3 Burger robot using ROS Noetic and Niryo Ned. It integrates the control systems of both robots, allowing for seamless operation and manipulation.

### Key Features
- Teleoperation of TurtleBot3 Burger in a simulated environment.
- Control integration with Niryo Ned for enhanced manipulation capabilities.
- User-friendly interface for easy operation.

## Getting Started
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites
- Ubuntu 20.04
- ROS Noetic
- Python 3
- Gazebo (for simulation)
- Pygame (Python library)

### Installation
1. Clone the repository into your ROS workspace (e.g., `catkin_ws`):
```bash
cd ~/tur_ws/src
git clone https://github.com/Greg7900/TurtleBot3_Niryo_Teleop.git
cd ..
catkin build
```

2. Install the necessary ROS dependencies:
```bash
rosdep install --from-paths src --ignore-src -r -y
```

3. Install Python dependencies:
```bash
pip install pygame
```

### Running the Simulation
To launch the TurtleBot3 Burger and Niryo Ned simulation, use the following commands:

1. Launch the desktop Gazebo simulation:
```bash
roslaunch tur_niryo_manipulator desktop_gazebo_simulation.launch
```

2. In a new terminal, navigate to the project's node directory and run the main script:
```bash
cd tur_ws/src/tur_niryo_manipulator/nodes
python3 robot_ned
```

## Usage
Once both the simulation and the script are running, you can teleoperate the TurtleBot3 Burger using the interface provided by the Niryo Ned system.


## Authors
- Your Name - *Initial work* - [Greg7900](https://github.com/Greg7900)

## Acknowledgments
- Moi
