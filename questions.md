### 1. Differences Between Reinforcement Learning and Evolutionary Algorithms
1) Reinforcement learning uses the concept of one agent, and the agent learns by interacting with the environment in different ways. In evolutionary algorithms, they usually start with many "agents" and only the "strong ones survive" (the agents with characteristics that yield the lowest loss).

2) Reinforcement learning agent(s) learns both positive and negative actions, but evolutionary algorithms only learns the optimal, and the negative or suboptimal solution information are discarded and lost.

Example

You want to build an algorithm to regulate the temperature in the room.

The room is 15 °C, and you want it to be 23 °C.

Using Reinforcement learning, the agent will try a bunch of different actions to increase and decrease the temperature. Eventually, it learns that increasing the temperature yields a good reward. But it also learns that reducing the temperature will yield a bad reward.

For evolutionary algorithms, it initiates with a bunch of random agents that all have a preprogrammed set of actions it is going to do. Then the agents that has the "increase temperature" action survives, and moves onto the next generation. Eventually, only agents that increase the temperature survive and are deemed the best solution. However, the algorithm does not know what happens if you decrease the temperature.

TL;DR: RL is usually one agent, trying different actions, and learning and remembering all info (positive or negative). EM uses many agents that guess many actions, only the agents that have the optimal actions survive. Basically a brute force way to solve a problem.
