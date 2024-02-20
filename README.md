# MDP REPRESENTATION

## AIM:
To represent any one real-world problem in MDP form.

## PROBLEM STATEMENT:

### Problem Description
Develop a robotic navigation game where the agent moves through levels (L1, L2, L3) taking actions (Forward, Backward, Stay), earning rewards based on successful navigation, and aiming to maximize the cumulative reward in a Markov Decision Process.

### State Space
The state space corresponds to different configurations or locations of the robot in the environment.
{L1, L2, L3} -> {0, 1, 2}

### Sample State
L1 -> 0 -> Level 1

### Action Space
The action space represents the robot's movement options.
{Forward, Backward, Stay} -> {0, 1, 2}

### Sample Action
Forward -> 0 -> Moving Forward

### Reward Function
The reward function assigns immediate rewards to the robot based on its actions and the resulting state.
Reward(State, Action, NextState)

### Graphical Representation
![1](https://github.com/manojvenaram/mdp-representation/assets/94165064/bf224b74-46d2-4c43-800b-082e82b0a826)


## PYTHON REPRESENTATION:

```python
Register Number:212221240025
Name: Manoj Choudhary V
T = {
    'L1': {
        'Forward': [(1.0, 'L2', 1.0, False)],
        'Stay': [(1.0, 'L1', 0.0, False)]
    },
    'L2': {
        'Forward': [(0.8, 'L3', 1.0, True), (0.2, 'L2', 0.0, False)],
        'Backward': [(1.0, 'L1', -1.0, False)]
    },
    'L3': {
        'Stay': [(1.0, 'L3', 0.0, True)],
        'Backward': [(1.0, 'L2', -1.0, False)]
    }
}
```

## OUTPUT:
![image](https://github.com/manojvenaram/mdp-representation/assets/94165064/d78f9291-cde1-410a-b290-3cf8da0d703b)


## RESULT:
Thus the given real world problem is successfully represented in a MDP form .

