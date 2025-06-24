MADDPG Financial Simulation
A realistic personal finance simulation using multi-agent reinforcement learning. This project uses MADDPG (Multi-Agent Deep Deterministic Policy Gradient) to train two AI agents with opposite spending habits: a smart budgeter and an impulsive spender.

Overview
I built a simple but smart environment to represent daily life money decisions. Each day, both agents decide how much to spend based on their emotional state, needs, and temptations.
The MADDPG algorithm helps both agents learn from experience — over time, they adjust their choices to try and be happier or richer (or both).

Goal
Simulate how different money behaviors affect life over time
Use AI agents that learn through trial and error
Show how emotions and financial choices are connected
Visualize progress with easy-to-understand graphs

How It Works
Custom Environment: BudgetingEnv
Each agent sees 7 inputs: account balance, happiness, cost of food, fuel, fun index, temptation level, and the current day
Action: Spend more or less (value between 0 and 1)
Reward: Based on a mix of happiness, savings, and avoiding overspending
Agents: Budgeter & Impulse Buyer
Each agent has:
An actor (decides what to do)
A critic (evaluates decisions)
They learn together using MADDPG
Noise is added so they explore new strategies
Learning Process
Experience is stored in memory
The agent learns by randomly picking past experiences and adjusting its brain (neural network)
Learning happens slowly (soft updates)

What Makes This Unique
Uses real feelings like regret and joy in the reward formula
Two agents interacting in the same world with different goals
Built from scratch environment to simulate financial life
Beautiful graphs show agent behavior and performance
Uses MADDPG which is advanced and realistic for group learning

Visual Outputs
Daily happiness of each agent
Daily balance changes
Reward chart for 30 days
Table showing final reward for both agents

Tools Used
Python
PyTorch
NumPy
Pandas
Matplotlib
OpenAI Gym (custom)

How to Use
Open MADDPG-Financial-Simulation.ipynb in Google Colab or Jupyter
Run each cell in order
See the training, results, and graphs

Sample Output
Episode
Budgeter
Impulse Buyer
1
963.48
-912.13
2
944.61
-1072.17
...
...
...

Budgeter learns to save. Impulse Buyer ends up with regrets.

Project Files
├── MADDPG-Financial-Simulation.ipynb  # Full code and graphs
├── README.md                          # Project summary (this file)

Ideas for Future
Add new types of agents (Investor, Minimalist, etc.)
Add emotional states like stress and regret
Use real spending data
Build a simple web app to play with it

Creator
Anjana
Graduate student in AI/ML, passionate about human-like AI simulations
