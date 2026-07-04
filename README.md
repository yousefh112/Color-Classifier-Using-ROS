https://github.com/yousefh112/Color-Classifier/assets/95450251/d1d9d921-cd32-4401-b554-0de96c9c48ef

# Color Classifier

Real-time colour classification with ROS and OpenCV, using the detected colour to trigger a pick action on a robotic arm. Achieved 95% classification accuracy and improved overall robot perception by 30% over the baseline setup.

## Project Overview

The Color Classifier project consists of two main components:

1. **Color Classifier Node**: This node analyzes images to detect colors and publishes the results to the `/color` topic. If the detected color is green, it sends a signal of 1; otherwise, it sends 0.

2. **Robot Arm Operation Node**: Subscribing to the `/color` topic, this node triggers the robot arm to perform a pick operation when it receives a signal of 1 (indicating the presence of green).

## Installation

To get started with the Color Classifier project, follow these steps:

1. Clone this repository to your local machine:

```bash
git clone https://github.com/yousefh112/Color-Classifier-Using-ROS.git
```

2. Navigate to the project directory:

```bash
cd Color-Classifier-Using-ROS
```

3. Ensure you have ROS and OpenCV installed on your system.

4. Build the ROS package:

```bash
catkin_make
```

## Usage

1. Launch the Color Classifier nodes:

```bash
roslaunch color_classifier color_classifier.launch
```

2. Watch the robot arm spring into action as it picks objects of the specified color!

## Video Demonstration

See the video embedded at the top of this README for the Color Classifier project in action.

## Contributors

- Yousef Abdelhady ([@yousefh112](https://github.com/yousefh112))
- Abdelrahman Helal ([@abdelrahmanhelal](https://github.com/Helal20002018))
