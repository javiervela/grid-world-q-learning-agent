# GridWorld Q-Learning Agent

A Reinforcement Learning agent implementing the Q-Learning algorithm to navigate and solve the GridWorld environment. The agent learns optimal policies through trial-and-error interactions with the environment, maximizing cumulative rewards.

> This project is an assignment for the course "Reinforcement Learning" at the Master in Artificial Intelligence Research at the Universidad Internacional Menéndez Pelayo (UIMP).

This repository builds upon a project from [RLCode](https://github.com/rlcode/reinforcement-learning), which is distributed under the MIT License. The original work has been adapted and extended to suit the objectives of this assignment.

## Requirements

- Python 3.13
- Poetry (https://python-poetry.org/)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/javier/grid-world-q-learning-agent.git
    cd grid-world-q-learning-agent
   ```
2. Install dependencies using Poetry:
   ```bash
    poetry install
   ```

### Usage

To start the learning environment with default settings, use the following command:

```bash
poetry run python q_learning_agent.py
```

By default, the agent will run for 50 episodes in a deterministic environment with a visualization of the learning process.

### Command-Line Options

You can customize the behavior of the agent using the following options:

- **`-s` (skip)**: Disables the full visualization of the learning process and only displays the final result.
- **`-e numEpisodes`**: Sets the number of episodes to run. The default is 50.
- **`-n noise`**: Specifies the probability (as a fraction) that the agent's actions deviate from the intended ones. The default is `0.0` (deterministic environment). A value greater than `0.0` introduces randomness, creating a stochastic environment.

For more details, run:

```bash
poetry run python q_learning_agent.py -h
```
