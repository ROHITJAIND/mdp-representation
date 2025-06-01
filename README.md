# MDP REPRESENTATION

## AIM:

To represent a Markov Decision Process(MDP) problem in the following ways.

    Text representation

    Graphical representation

    Python - Dictonary representation

### PROBLEM STATEMENT:

The agent has to reach AR/VR (EEE) lab starting from admin 5th floor. The floor is slippery and the agent has 2 options either to move left or right. Probabillity of moving the desired direction is 0.8.

### State Space

0 : Admin

1 : CSE

2 : ECE

3 : EEE(AR/VR)

### Sample State

The agent is at CSE state -> 1.

### Action Space

Left : 0

Right : 1

### Sample Action

The agent takes left from the current state -> 0.

### Reward Function

R = {+1 if state = 3}

### Graphical Representation

![](1.png)

## PYTHON REPRESENTATION:

```
p = {
    0:{
        0:[(0.8, 1, 0, False), (0.2, 2, 0, False)],
        1:[(0.8, 2, 0, False), (0.2, 1, 0, False)]
    }
    1:{
        0:[(0.8, 1, 0, False), (0.2, 0, 0, False)],
        1:[(0.8, 0, 0, False), (0.2, 1, 0, False)]
    }
    2:{
        0:[(0.8, 0, 0, False), (0.2, 3, 1, True)],
        1:[(0.8, 3, 1, True), (0.2, 0, 0, False)]
    }
}
```

## OUTPUT:

![](op1.png)

## RESULT:

Thus the given Markov Decision Process(MDP) problem is represented in the following ways.

Text representation

Graphical representation

Python - Dictonary representation
