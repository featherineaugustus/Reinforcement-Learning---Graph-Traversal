# Reinforcement-Learning---Graph-Traversal

We illustrate the concept of Q-learning via a graph traversal search. 

From a starting node, we traverse to a specific node (goal).

- Agent: Robot
- Environment: Graph
- State: Position of the Robot in the Graph
- Action: Movement (traversal)
- Reward: 100 at goal, 0 otherwise

Variables:
- Q : Estimated Policy Table
- M : True Reward Table
- $\gamma$ : Learning Rate

This project is extended from: 

https://www.geeksforgeeks.org/ml-reinforcement-learning-algorithm-python-implementation-using-q-learning/


Originally, the project estimate Q by:
1) Begin at a random node, and check the best possible route to transverse to via Q.
2) We update Q = M + $\gamma$*(current reward).
3) Repeat for another random node.

However, this approach may initialize the random node to the goal node, where we will attempt to traverse out of the goal, which is counterintuitive.

Instead, we should:
1) Begin at the start node, and attempt to transverse to the goal node via Q.
2) We update Q along the way, such that the routes closer to the goal is grant larger rewards.
3) We restart to the start node once we reached the goal node.

This approach is more intuitive, which is better for an illustration for Q-learning.

Feel free to explore and edit the code accordingly.

