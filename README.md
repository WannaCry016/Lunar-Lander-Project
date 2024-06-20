# Lunar Lander

![Lunar Lander](./images/lunar_lander.gif)

This project uses Deep Q-Learning to train an agent to land a lunar lander safely on a landing pad on the surface of the moon.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Training Details](#training-details)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This project involves using the [OpenAI Gym](https://gym.openai.com/) environment to simulate the Lunar Lander game. The agent is trained using a Deep Q-Network (DQN) to navigate and land the lunar module using reinforcement learning.

## Features

- Implementation of Deep Q-Learning with Experience Replay.
- Interaction with the Gym environment to train and test the agent.
- Visualization of the training process and the performance of the trained agent.

## Installation

1. Clone this repository:
    ```bash
    git clone https://github.com/yourusername/lunar-lander.git
    cd lunar-lander
    ```

2. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

3. You may also need to set up a virtual display for rendering:
    ```bash
    sudo apt-get install xvfb
    ```

## Usage

1. To train the agent, open the Jupyter Notebook `TensorFlow - Lunar Lander.ipynb` and run all cells. Make sure to follow the instructions in the notebook for setting up the environment and running the training process.

2. To visualize the trained agent in action, execute the notebook cells in section "See the Trained Agent In Action."

## Project Structure

```plaintext
lunar-lander/
│
├── images/
│   └── lunar_lander.gif
│
├── utils/
│   └── utils.py
│
├── Lunar_Lander.ipynb
├── requirements.txt
└── README.md
```

- `images/`: Contains images used in the README and notebook.
- `utils/`: Contains helper functions and utilities for the project.
- `Lunar_Lander.ipynb`: Main Jupyter Notebook for training and testing the agent.
- `requirements.txt`: List of dependencies for the project.
- `README.md`: Project documentation.

## Training Details

### Environment

The Lunar Lander environment from OpenAI Gym has:
- **Action Space**: Discrete actions to control the lander's engines.
- **Observation Space**: Continuous state space representing lander's position, velocity, angle, and angular velocity.
- **Rewards**: Positive reward for successful landing and penalties for crashing or excessive fuel consumption.

### Algorithm

- **Deep Q-Learning**: Uses a neural network to approximate the Q-value function, which is updated during training to minimize the difference between predicted and target Q-values.
- **Experience Replay**: Stores past experiences and samples them randomly to break correlation in training data.

## Results

The trained agent learns to land the lunar module by maximizing the reward signal from the environment. After sufficient training, the agent is capable of consistently achieving successful landings.

## Contributing

Contributions are welcome! Please fork this repository, create a branch for your changes, and submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---


