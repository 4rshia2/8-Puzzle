# 8-Puzzle Solver
This Python program is designed to solve the classic 8-puzzle problem using various search algorithms. The 8-puzzle is a sliding puzzle that consists of eight numbered tiles and an empty space on a 3x3 grid. The objective is to rearrange the tiles into their correct order using the fewest possible moves.

## Search Algorithms Implemented
The program implements the following search algorithms to solve the 8-puzzle problem:

1. Depth-First Search (DFS):

    Depth-First Search explores as far as possible along a branch before backtracking.
The program finds a solution by iteratively exploring possible moves in a depth-first manner.

2. Iterative Deepening Search (IDS):

    Iterative Deepening Search is a combination of depth-first search and breadth-first search.
The program performs multiple depth-limited searches, gradually increasing the depth limit, until a solution is found.

3. Breadth-First Search (BFS):

    Breadth-First Search explores all the neighbor nodes at the current depth before moving to the next level.
The program explores possible moves in a breadth-first manner to find the solution.

4. Uniform Cost Search (UCS):

    Uniform Cost Search explores the node with the lowest path cost first.
The program uses this algorithm to find the optimal solution.

5. A Search:*

    A* Search is an informed search algorithm that uses a heuristic to estimate the cost of reaching the goal.
The program combines the Manhattan distance heuristic with UCS to find an optimal solution.

## Usage
To use the program, input the initial state of the 8-puzzle as a list of comma-separated values, where 0 represents the empty tile. For example:
```
Enter the initial state of the 8-puzzle (comma-separated values): 2, 8, 3, 1, 6, 4, 7, 0, 5
```
The program will then apply each of the above search algorithms and output the following:

* The sequence of moves to solve the puzzle.
* The total time taken to find a solution (in milliseconds).
* Memory usage for each algorithm (in bytes).

## Memory and Time Analysis
The program uses Python's tracemalloc and the time module to perform memory and time analysis for each search algorithm. This information helps you evaluate the efficiency of each algorithm in terms of memory consumption and execution time.

