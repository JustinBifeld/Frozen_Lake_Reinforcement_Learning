# Frozen_Lake_Reinforcement_Learning
The goal of this repository is to create a Q-Learning agent to play the game Frozen Lakes from OpenAI Gym.  A large amount of inspiration and guidance for this 
came from [deeplizard](https://deeplizard.com/).  The Frozen Lakes game is describe on [OpenAI Gym's website](https://gym.openai.com/envs/FrozenLake-v0/) as:

Winter is here. You and your friends were tossing around a frisbee at the park when you made a wild throw that left the frisbee out in the middle of the lake. The water is mostly frozen, but there are a few holes where the ice has melted. If you step into one of those holes, you'll fall into the freezing water. At this time, there's an international frisbee shortage, so it's absolutely imperative that you navigate across the lake and retrieve the disc. However, the ice is slippery, so you won't always move in the direction you intend.
The surface is described using a grid like the following:
SFFF       (S: starting point, safe)  
FHFH       (F: frozen surface, safe)  
FFFH       (H: hole, fall to your doom)  
HFFG       (G: goal, where the frisbee is located)
The episode ends when you reach the goal or fall in a hole. You receive a reward of 1 if you reach the goal, and zero otherwise.

This implementation uses a Q-Table to represent our state spaces and action spaces.  The states are every tile in the game (16 in total) and the actions are the possible moves (up, down, left, right).  This serves as a great introduction to reinforcement learning and specifically Q-learning.  Below you can see what the game looks like when the program plays it and reaches the goal.

