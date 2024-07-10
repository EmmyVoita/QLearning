# QLearning

This project demonstrates the implementation of a Q-learning algorithm to solve a grid-based pathfinding problem in Unity. The solver navigates an agent through a grid, avoiding obstacles and maximizing rewards based on a predefined reward table.

**Features**
- Q-Learning Algorithm: Implements Q-learning with adjustable parameters such as learning rate (alpha), discount factor (gamma), and exploration rate (epsilon).
- Grid-Based Pathfinding: Solves pathfinding problems in a grid environment with obstacles.
- Flexible Configuration: Allows for customization of grid size, obstacle positions, and reward structures.
- State and Action Management: Manages state transitions, rewards, and Q-values for effective learning and decision-making.
- Policy Extraction: Extracts optimal policies at regular intervals for evaluation and analysis.

**Components**
Agent: Controls the agent's movement within the grid.
QLearningSolver: Handles the Q-learning algorithm, including state transitions, rewards, and Q-value updates.
MDP: Defines the Markov Decision Process (MDP) with transition probabilities and rewards.

**How to Use**
Setup the Grid: Define the grid size, obstacle positions, and reward table.
Configure Q-Learning Parameters: Set the learning rate (alpha), discount factor (gamma), and exploration rate (epsilon) in the QLearningSolver script.
Run Training: Execute the Q-learning training process to learn optimal policies.
Evaluate Policies: observe the agent's behavior at training intervals.

**KeyBinds**
"space" increments the episode number and puts the agent at a random start state
"c" puts the agent at a random start state and maintains the episode number
"x" puts the agent at a defined start state (defined in the Unity editor) and maintains the episode number


![image](https://github.com/EmmyVoita/QLearning/assets/82542924/49f463d7-c436-458a-b88a-b42b860fda43)


The included zip file is a unity project that implements Q-learning using temporal difference. It is created with Unity 2021.3.9f1, but should work fine with other versions. The scripts that implement Q-Learning are as follows:

"UnityProject\Assets\NewScripts\QLearningMain.cs"

- Calls the Q-learning function and sets up the mover.

"UnityProject\Assets\NewScripts\QLearningSolver.cs"

- Contains the functions for implementing Q-learning, getting the optimal policy, setting the reward and transition arrays, and other helper functions.

"UnityProject\Assets\NewScripts\Mover.cs"

- Moves the agent in the scene based on the optimal policy

