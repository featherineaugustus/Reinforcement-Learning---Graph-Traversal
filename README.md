# Reinforcement-Learning---Graph-Q-Learning

# Graph Q-Learning

We illustrate the concept of Q-Learning via a graph network search. From a starting node, we wish to transverse the agent to a specific node (goal).

Q -> Estimated Reward Table
M -> True Reward Table
$\gamma$ -> Learning Rate

We utilized a random initalization process to estimate Q. 
1) We randomly begin at a node and check the best possible route to transverse via Q.
2) We update Q = M + $\gamma$*(current reward).
3) Repeat for another random node.

Another possible method is to:
1) We begin at the start, and attempt to transverse to the goal via Q.
2) We update Q along the way, such that the routes closer to the goal is grant larger rewards.

Feel free to explore and edit the code accordingly.

This project is extended from: 
https://www.geeksforgeeks.org/ml-reinforcement-learning-algorithm-python-implementation-using-q-learning/
