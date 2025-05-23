## 🎮 Tetris AI with Deep Q-Learning

This project implements a reinforcement learning agent that learns to play the game of **Tetris** using a **Deep Q-Network (DQN)** approach. The agent is trained from scratch and learns optimal moves through interaction with the Tetris environment.

### 📁 Project Structure

```
JavisyH/
├── train.py                # Training loop using DQN
├── test.py                 # Script to evaluate the trained model
├── src/
│   ├── tetris.py           # Tetris game logic and environment
│   ├── deep_q_network.py   # Neural network architecture for the DQN
├── tensorboard/
│   └── events.out.*        # Logs for training visualization in TensorBoard
├── trained_models/
│   └── tetris              # Trained model weights
```

### 🚀 How to Run

1. **Install Requirements**:

   ```bash
   pip install -r requirements.txt
   ```

2. **Train the Agent**:

   ```bash
   python train.py
   ```

3. **Evaluate the Model**:

   ```bash
   python test.py
   ```

4. **Visualize Training** (optional):

   ```bash
   tensorboard --logdir=tensorboard
   ```

### 🧠 Model

The Deep Q-Network (DQN) consists of a fully connected neural network that maps Tetris board states to Q-values representing the expected reward of each possible action.

### 🎯 Features

* Custom Tetris environment (`tetris.py`)
* Deep Q-Learning with experience replay
* TensorBoard logging for training progress
* Pretrained model saving and loading

### 📌 Notes

* The model performance may depend on training time and hyperparameter tuning.
* Works best with GPU acceleration for faster training.

