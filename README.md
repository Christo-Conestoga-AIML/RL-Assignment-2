

# Assignment 2 - Q-Learning on Taxi-v3
| Student Name           | Student Id | Course                                        |
|------------------------|------------|-----------------------------------------------|
| Christo Pananjickal Baby | 8989796    | CSCN8020 - Reinforcement Learning Programming |

### Intro

This assignment demonstrates how the **Q-Learning algorithm** can be used to train an agent in the **Taxi-v3** environment from OpenAI Gym. The agent learns to pick up and drop off passengers efficiently through exploration and exploitation. The assignemt already comes with an helper file `lib/assignment2_utils.py` which contains functions to describe the environment, simulate the episodes etc.

### Environments and rewards
The Taxi-v3 environment simulates a grid world where the agent must pick up and drop off passengers at specific locations.
Rewards are given for successful drop-offs (+20) and penalized for wrong pickups or illegal moves (-10 or -1 per step).

### What assignment includes 
- Implemented a reusable Q-Learning training function.
- Logged detailed steps for the first few episodes to show how the Q-table updates.
- Tracked metrics such as training time, average reward, and total steps per episode.
- Conducted experiments by changing **learning rate (α)** and **discount factor (γ)** values to observe their effects.
- Visualized training progress using line graphs of episode rewards.

### Parameters Tested
- **Learning Rate (α):** 0.01, 0.001, 0.2  
- **Discount Factor (γ):** 0.2, 0.3  
- **Baseline:** α = 0.1, γ = 0.9  

###  Evaluation Metrics
- Training Time (s)  
- Average Return per Episode  
- Total Steps per Episode  
- Total Episodes  
- Learning Rate, Exploration Factor, Discount Factor  

### How to Run the Code
1. Clone this repo using
    ```bash
    git clone https://github.com/Christo-Conestoga-AIML/RL-Assignment-2.git
2. Navigate to the cloned folder.
    ```bash
    cd RL-Assignment-2
3. Make sure you are using python 3.12
4. Create and activate a virtual environment:
   ```bash
   python3 -m venv .venv
   .venv\Scripts\activate
5. Install the required dependencies from `requirements.txt`
   ```bash
   pip install -r requirements.txt
6. Open and run the notebook `lib/main.ipynb` sequentially
   