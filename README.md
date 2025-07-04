# autoTaxi

## Overview
autoTaxi is a reinforcement learning project that uses Double Q-Learning to solve the OpenAI Gym Taxi-v3 environment. The agent learns to efficiently pick up and drop off passengers in a grid world using two Q-tables to reduce overestimation bias.

## Features
- Double Q-Learning implementation for Taxi-v3
- Training with reproducibility (fixed random seed)
- Logging of training progress and episode results
- Saving and loading of Q-tables
- Evaluation with human-rendered environment

## Project Structure

```
autoTaxi/
  Double_QN_autoTaxi.ipynb   # Main Jupyter notebook with code and experiments
  taxi_qtable1.npy           # Saved Q-table 1 (numpy array)
  taxi_qtable2.npy           # Saved Q-table 2 (numpy array)
  taxi_training_log.txt      # Log file with episode results
README.md                    # Project documentation
```

## Getting Started

1. **Install dependencies:**
   - Python 3.8+
   - numpy
   - gymnasium

   You can install dependencies with:
   ```bash
   pip install numpy gymnasium
   ```

2. **Run the notebook:**
   Open `Double_QN_autoTaxi.ipynb` in Jupyter and run all cells to train and evaluate the agent.

3. **View logs and results:**
   - Training progress and episode results are saved in `taxi_training_log.txt`.
   - Final Q-tables are saved as `.npy` files for reuse or further analysis.

## How It Works

The notebook implements Double Q-Learning, which maintains two Q-tables and updates them alternately to reduce overestimation. The agent is trained for a large number of episodes, and its performance is evaluated in a human-rendered environment after training.

## References
- [OpenAI Gymnasium: Taxi-v3](https://gymnasium.farama.org/environments/toy_text/taxi/)
- [Double Q-Learning Paper](https://www.aaai.org/Papers/AAAI/2010/AAAI10-106.pdf)
