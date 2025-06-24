# smart-vs-spender-maddpg
A Multi-Agent Reinforcement Learning simulation using MADDPG where two AI agents — a budgeter and an impulsive spender — learn competing strategies to manage daily expenses over time.
This simulation builds a custom multi-agent environment using OpenAI Gym where:
Each agent starts with the same balance and happiness score
Actions represent daily spending decisions
Rewards depend on remaining balance, happiness gain, and emotional penalties
Agents learn and evolve spending behavior across 30 simulated days per episode
We trained these agents using the MADDPG algorithm, where each agent:
Has its own actor-critic networks
Learns based on both its state and the other agent’s behavior
Updates through centralized training but acts independently during inference
What Makes This Project Special?

Most budgeting simulations are either simple or focus on one agent. This project is different because:

Adds emotional dynamics like happiness curves and regret from overspending

Builds a custom Gym environment for financial behavior

Uses MADDPG for training multiple agents who compete and learn together

 Tracks training over time with detailed rewards

 Includes clear graphs showing how agents evolve their strategies
