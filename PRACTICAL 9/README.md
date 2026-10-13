# PRACTICAL 9

## Title

Implementation of Goal Stack Planning in Artificial Intelligence using Python.

## Aim

To implement a goal-based planning system in Python that finds a sequence of actions to achieve a specified goal from an initial state.

## Objective

* To understand the concept of goal-based planning in Artificial Intelligence.
* To represent actions using preconditions, add lists, and delete lists.
* To generate a plan by satisfying the preconditions of actions.
* To achieve the goal state from the initial state.

## Theory

Goal Stack Planning is an AI planning technique used to find a sequence of actions required to achieve a particular goal. It works by identifying an action that can achieve the goal, satisfying its preconditions, and then executing the action.

In this program, the initial state is `At_A`, and the goal is `At_C`. Two actions are defined:

1. **Move A to B:** Moves the object from location A to location B.
2. **Move B to C:** Moves the object from location B to location C.

Each action contains three components:

* **Preconditions (`pre`):** Conditions that must be true before executing an action.
* **Add list (`add`):** Facts that become true after executing the action.
* **Delete list (`delete`):** Facts that become false after executing the action.

The program recursively satisfies the preconditions and executes the required actions to reach the goal.

## Algorithm

1. Initialize the state with `At_A`.
2. Define the goal as `At_C`.
3. Define actions with their preconditions, add lists, and delete lists.
4. Find an action that can achieve the given goal.
5. Check whether the goal is already true in the current state.
6. Recursively satisfy the preconditions of the selected action.
7. Execute the action by updating the current state.
8. Add the action name to the plan.
9. Repeat until the goal is achieved or no suitable action is found.
10. Display the generated plan.

## Expected Output

```text
Plan:
Move A to B
Move B to C
```

## Result

Thus, the Goal Stack Planning program was implemented successfully in Python. The program generates a sequence of actions to move from location A to location C and achieve the specified goal.
