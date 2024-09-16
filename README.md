![preview](https://github.com/user-attachments/assets/70689ec4-8afe-49f7-b8ed-6e3a32dd8a6d)
# Drive-AI-race-car-
Here’s a sample README file for your car simulation project using NEAT and Pygame. This README provides an overview of the project, installation instructions, usage, and any relevant details.

---

# Car Simulation with NEAT and Pygame

## Overview

This project simulates a car navigating a track using a neural network evolved with the NEAT (NeuroEvolution of Augmenting Topologies) algorithm. The simulation is built using Python's Pygame library for visualization and NEAT-Python for evolving neural networks.

## Features

- **Car Navigation**: The car uses a neural network to navigate the track, adjusting its direction to avoid collisions.
- **Collision Detection**: The simulation detects collisions with the track's borders and stops the car if a collision occurs.
- **Radar System**: The car has a radar system that detects the distance to obstacles in different directions.

## Installation

1. **Clone the Repository**

   ```sh
   git clone https://github.com/yourusername/your-repository.git
   cd your-repository
   ```

2. **Install Dependencies**

   Make sure you hav![preview](https://github.com/user-attachments/assets/85fa7230-f221-4f77-9dc9-6dd4b274a7ec)
e Python 3.12 or higher installed. Install the required packages using pip:

   ```sh
   pip install pygame neat-python
   ```

3. **Add Assets**

   Place your track and car images in the `Assets` directory. The expected file names are `track.png` and `car.png`.

## Usage

1. **Configure NEAT**

   Make sure you have a configuration file for NEAT named `config.txt` in the project directory. This file contains the parameters for the NEAT algorithm. You can modify this file to tweak the neural network's evolution settings.

2. **Run the Simulation**

   Execute the `diffmap.py` script to start the simulation:

   ```sh
   python diffmap.py
   ```

   This will initialize the NEAT algorithm and start the car simulation on the track. The simulation will run for 50 generations, as specified in the `pop.run(eval_genomes, 50)` call.

## Code Overview

- **`Car` Class**: Defines the car's properties, behavior, and methods for movement, collision detection, rotation, and radar functionality.
- **`remove` Function**: Removes cars, genomes, and networks from the simulation when a car collides or is otherwise no longer active.
- **`eval_genomes` Function**: Evaluates each genome by running the simulation and updating the fitness of each genome based on the car's performance.
- **`run` Function**: Sets up the NEAT configuration and runs the evolutionary process.

## Troubleshooting

- **IndexError: pixel index out of range**: This error usually occurs if the car's radar or collision detection is trying to access a pixel outside the bounds of the track image. Ensure your track image is properly loaded and its dimensions are appropriate.
- **SyntaxError: (unicode error) 'unicodeescape' codec**: This is a common issue with file paths on Windows. Use raw strings (`r"your_path"`) or double backslashes (`"C:\\path\\to\\file"`).

## Contributing

Feel free to contribute to this project by submitting issues or pull requests. Improvements, bug fixes, and feature enhancements are welcome.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

