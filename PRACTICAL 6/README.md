# Map Coloring Using Backtracking

## Description

This program solves the **Map Coloring Problem** using the **Backtracking Algorithm**.

The objective is to assign a color to each region of a map such that no two neighboring regions have the same color.

The program uses three colors:

* Red
* Green
* Blue

The map contains four regions:

* A
* B
* C
* D

Each region has neighboring regions defined in the `map_data` dictionary.

## Algorithm Used

The program uses **Backtracking** to find a valid coloring.

### Steps

1. Select an uncolored region.
2. Try assigning one of the available colors.
3. Check whether the selected color conflicts with any neighboring region.
4. If there is no conflict, assign the color.
5. Continue with the next region.
6. If no color is possible, undo the previous assignment and try another color.
7. Continue until all regions are successfully colored.

## Functions

### `is_consistent(region, color, assignment)`

Checks whether assigning a particular color to a region is valid.

It compares the color with the colors already assigned to its neighboring regions.

### `solve_map(assignment)`

Uses recursive backtracking to assign colors to all regions.

If a valid solution cannot be found for the current assignment, the function backtracks and tries another color.

## Input

The program uses the following map:

```python
map_data = {
    'A': ['B', 'C'],
    'B': ['A', 'C', 'D'],
    'C': ['A', 'B', 'D'],
    'D': ['B', 'C']
}
```

Available colors:

```python
colors = ['Red', 'Green', 'Blue']
```

No user input is required.

## Output

The program prints the color assigned to each region.

Example:

```text
Solution:
A = Red
B = Green
C = Blue
D = Red
```

The exact valid assignment may depend on the order in which regions and colors are processed.

## Requirements

* Python 3.x
* No external libraries are required.

## How to Run

1. Save the program as:

```text
map_coloring.py
```

2. Open a terminal or Python IDE.
3. Run:

```bash
python map_coloring.py
```

## Concepts Used

* Backtracking
* Recursion
* Constraint Satisfaction Problem (CSP)
* Graph Coloring
* Dictionaries
* Lists
* Functions

## Applications

Map coloring is a common example of a **Constraint Satisfaction Problem** and can be applied to:

* Geographic map coloring
* Timetable scheduling
* Register allocation
* Frequency assignment
* Resource allocation

## Conclusion

This program demonstrates how the **Backtracking Algorithm** can be used to solve a map coloring problem by systematically assigning colors and undoing assignments whenever a conflict occurs.
