# Gravis Robot

Welcome to the official repository for Gravis, an innovative autonomous robot designed to redefine indoor navigation. Gravis combines cutting-edge technology and robust hardware components to navigate complex environments with precision and adaptability.

## Technologies & Components

Gravis is engineered with a blend of Raspberry Pi 4 and Arduino at its core, facilitating seamless control and integration of various sensors and actuators. Key components include:

- **Raspberry Pi 4**: Serves as the brain of Gravis, handling high-level processing and decision-making.
- **Arduino**: Manages real-time control of motors and reads sensor data, ensuring responsive and reliable operation.
- **RPLidar A1**: Offers 2D mapping capabilities, enabling Gravis to understand and navigate its surroundings efficiently.
- **Metal Chassis**: A robust framework designed for durability, capable of withstanding challenging off-road conditions.
- **Modular Grid Design**: Provides unparalleled flexibility, allowing for easy customization and upgrades.
- **All-Terrain Tank Tracks**: Ensures Gravis can traverse various surfaces, from smooth floors to rugged terrains.
- **User-Friendly Interface**: Simplifies interaction, making Gravis accessible to users of all skill levels.

## Project Scope

This repository is dedicated to implementing autonomous indoor navigation using the Robot Operating System (ROS) alongside the RPLidar A1 sensor. The focus is on developing algorithms and software components that enable Gravis to autonomously map and navigate indoor environments.

## Getting Started

### Prerequisites

- Raspberry Pi 4 (4GB or 8GB RAM version recommended)
- Arduino (Uno or Mega)
- RPLidar A1
- Compatible metal chassis and tank tracks
- Basic electronic components (wires, connectors, etc.)

### Installation

1. **Set Up Raspberry Pi**: Flash the latest version of Raspberry Pi OS onto your Pi. Ensure it's connected to the internet and updated (`sudo apt-get update && sudo apt-get upgrade`).

2. **Install ROS**: Follow the [official ROS installation guide](http://wiki.ros.org/ROS/Installation) for Raspberry Pi. We recommend ROS Noetic for compatibility.

3. **Arduino Setup**: Install the Arduino IDE and ensure it can communicate with your Arduino board. Load the provided motor control and sensor reading sketches.

4. **Clone the Repository**: Clone this repo to your Raspberry Pi.
   ```
   git clone [https://github.com/yourusername/gravis-robot.git](https://github.com/42dotmk/GravisRobotROS)
   ```

5. **Install Dependencies**: Navigate to the project directory and install required ROS packages and dependencies.
   ```
   cd gravis-robot
   rosdep install --from-paths src --ignore-src -r -y
   ```

### Usage

- **Calibration**: Follow the calibration guide in the `docs` directory to calibrate sensors and motors.
- **Launching Gravis**: Use the provided launch files to start Gravis's navigation system.
  ```
  roslaunch gravis_robot navigation.launch
  ```

## Contributing

We welcome contributions from the community, whether it's in the form of bug reports, feature requests, or pull requests. Please refer to our CONTRIBUTING.md for more information.

## License

This project is licensed under the GNU General Public License v3.0 - see the [LICENSE.md](LICENSE) file for details.
