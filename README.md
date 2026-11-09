# Q-Learning Agent for Taxi-v3 Navigation

Team project for Artificial Intelligence, supervised by Dr. Marzieh Zarrinbal at Amirkabir University of Technology.

## Learning and evaluation

The agent learns a tabular policy for Gym's Taxi-v3 simulation. The Q-table has 500 states and six actions. Training uses an epsilon-greedy policy with a learning rate of 0.1, discount factor of 0.99, and exploration probability of 0.1. The implementation applies a Bellman update after each transition and trains for 100,000 episodes.

The main script evaluates the greedy policy for 100 episodes, reporting average steps and penalties per episode. It also produces a heatmap of the Q-table. The random generator used to choose between exploration and exploitation is seeded. Episode resets and action-space sampling have separate random state, so the reported averages can vary across runs.

## Validation run

The original training script completed in a local validation environment with Gym 0.26.2 and NumPy 1.26.4. One run averaged 13.13 steps and 0.00 penalties per evaluation episode. These numbers describe that validation run.
