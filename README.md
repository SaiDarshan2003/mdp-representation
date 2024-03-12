# MDP REPRESENTATION

## AIM

To represent a Markov Decision Process(MDP) problem.

## PROBLEM STATEMENT:

### Problem Description

A robotic agent is tasked with navigating through an environment. The agent begins at the starting point (S) and aims to reach a targeted location (T) while avoiding obstacles (O). The agent has the ability to move forward (F) and backward (B) within the environment.

### State Space

S (Starting point): 0

M (Moving forward): 1

T (Targeted location): 2

O (Encountering obstacle): 3

### Sample State:

In the event of moving backward from the start position the robot will face an obstacle

### Action Space

F (Forward movement): 1

B (Backward movement): 2

### Sample Action

The robot takes forward movemnt to go from start state to forward state.

### Reward Function

+1 if the agent reaches the targeted location (T)

0 otherwise

### Graphical Representation

![image](https://github.com/SaiDarshan2003/mdp-representation/assets/94692595/9859006b-d4d0-47c8-a8bf-dd8a4890ce6a)

## PYTHON REPRESENTATION
```
Sai Darshan G
212221240047

robot_mdp = {
    0: {
        1: [(0.85, 1, 0, False), (0.15, 0, 0, False)],
        2: [(0.92, 0, 0, False), (0.08, 1, 0, False)]
    },
    1: {
        1: [(0.88, 2, 1, True), (0.12, 0, 0, False)],
        2: [(0.78, 0, 0, False), (0.22, 2, 1, True)]
    },
    2: {
        1: [(0.94, 2, 0, False), (0.06, 1, 0, False)],
        2: [(0.89, 1, 0, False), (0.11, 2, 0, False)]
    },
    3: {
        1: [(0.80, 3, 0, True), (0.20, 2, 0, False)],
        2: [(0.75, 2, 0, False), (0.25, 3, 0, True)]
    }
}
```

## OUTPUT

![image](https://github.com/SaiDarshan2003/mdp-representation/assets/94692595/46a87664-5efc-4304-9dba-38cf923322c6)


## RESULT

Above, We have represented an MDP problem in a textual,graphical and technical manner successfully.

