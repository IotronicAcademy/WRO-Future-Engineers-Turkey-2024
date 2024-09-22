# ![Logo](other/logo.jpeg) WRO-Future-Engineers-Turkey-2024


## Content

* `t-photos` contains 2 photos of the team (an official one and one funny photo with all team members).
* `v-photos` contains 6 photos of the vehicle (from every side, from top and bottom).
* `video` contains the video.md file with the link to a video where the driving demonstration exists.
* `schemes` contains one or several schematic diagrams in the form of JPEG, PNG, or PDF of the electromechanical components illustrating all the elements (electronic components and motors) used in the vehicle and how they connect to each other.
* `src` contains the code of control software for all components that were programmed to participate in the competition.
* `models` is for the files for models used by 3D printers, laser cutting machines, and CNC machines to produce the vehicle elements. If there is nothing to add to this location, the directory can be removed.
* `other` is for other files which can be used to understand how to prepare the vehicle for the competition. It may include documentation on how to connect to an SBC/SBM and upload files there, datasets, hardware specifications, communication protocols descriptions, etc. If there is nothing to add to this location, the directory can be removed.

## Introduction

The robot in question is equipped with a series of technological components designed to optimize its obstacle detection capabilities in this WRO robotics competition. Among its main features are three range sensors, a camera, an RGB line sensor, two motors with encoders, and two servos. Each of these elements plays a significant role in the robot's operation and maneuverability.

The range sensors are crucial for the robot's navigation. These sensors are strategically positioned to allow precise detection of obstacles in the robot's environment. Typically, range sensors operate by emitting ultrasonic waves or lasers that bounce back to the sensor upon hitting an object. This return is measured to determine the distance between the sensor and the obstacle. In the robot's case, the three range sensors are distributed such that one is oriented forward while the other two are positioned on the sides. This arrangement provides wide coverage of the environment, enabling the robot to detect obstacles not only directly in front of it but also around it. This is particularly useful for avoiding collisions with walls and other nearby objects. The front sensor provides information about obstacles directly in the robot's path, while the side sensors are essential for more complex maneuvers, such as turns or direction changes when encountering side obstacles.

The camera mounted on the robot serves a specific purpose related to obstacle color detection. This camera is equipped to identify two primary colors: red and green. The ability to detect the color of an obstacle allows the robot to make more informed decisions about its behavior. For instance, if the robot detects a red-colored obstacle, it may be programmed to avoid it differently than it would a green obstacle. The camera uses image processing to identify and distinguish these colors, which involves a series of algorithms that analyze the captured image to extract relevant information about the environment.

In addition to the range sensors and the camera, the robot is equipped with an RGB line sensor. This sensor is designed to detect specific colored lines on the ground, in this case, orange and blue. The primary function of the RGB line sensor is to allow the robot to follow predefined routes based on the colors detected on the ground. For example, if the robot is programmed to follow a blue line, the RGB sensor will identify that line and adjust the robot's movement to stay on it. This type of control is essential for applications where the robot must follow a specific path or avoid certain zones marked by colors.

As for the motors, the robot is equipped with two motors with encoders. Encoders are devices that provide precise feedback on the motors' speed and position, which is crucial for controlling the robot's movement. Encoders convert the rotational motion of the motors into digital signals that can be interpreted by the robot's control system. This allows fine adjustments to the robot's speed and direction, as well as greater precision in maneuvers. Motors with encoders enable the robot to move more controlled and precisely, facilitating navigation in complex environments and the execution of specific tasks.

The robot is also equipped with two servos, each with a distinct function. The first servo is connected to a wheel system responsible for steering the robot. This servo adjusts the angle of the wheels, allowing the robot to turn and change direction precisely. The ability to modify the wheel's direction is essential for the robot's maneuverability, enabling it to make turns and movements in different directions easily.

The second servo is intended to adjust the camera's angle. This adjustment capability is particularly useful for changing the perspective from which the robot is observing its environment. For example, the camera angle can be adjusted to obtain a clearer view of an obstacle or to change the camera's orientation based on the robot's needs at any given moment. Adjusting the camera angle allows for greater flexibility in detecting and analyzing the environment, adapting to different situations and navigation scenarios.

The robot was constructed using a Makeblock CiberPi, as it allows for functionalities that provide a better structure for the robot. The code compilation and upload process is done via USB-C or Bluetooth, and the program also allows for a preview without uploading the code, showing the programming in real time.

---
