
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
git clone [URL to your GitHub repository]
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
python3 robot_ned.py
```

## Usage
Once both the simulation and the script are running, you can teleoperate the TurtleBot3 Burger using the interface provided by the Niryo Ned system.

## Contributing
Please read [CONTRIBUTING.md](link-to-your-contributing-md-file) for details on our code of conduct, and the process for submitting pull requests to us.

## Authors
- Your Name - *Initial work* - [YourGitHubUsername](link-to-your-github-profile)

## License
This project is licensed under the [Your License] License - see the [LICENSE.md](link-to-your-license-file) file for details.

## Acknowledgments
- Hat tip to anyone whose code was used
- Inspiration
- etc
```

Remember to replace the placeholders (like `[URL to your GitHub repository]`, `[Your License]`, `Your Name`, `[YourGitHubUsername]`, `[link-to-your-license-file]`, and `[link-to-your-contributing-md-file]`) with the actual details relevant to your project.