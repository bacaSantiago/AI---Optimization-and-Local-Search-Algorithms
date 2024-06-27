# AI - Optimization and Local Search Algorithms

---

## Overview
This Python program implements local search algorithms such as Greedy Search, Random Walk, Hill Climbing, and Simulated Annealing to solve two distinct problems: the Eight Queens Puzzle and finding the optimal route among a collection of points on the plane. The primary goal is to compare the performance of different algorithms in terms of their ability to find optimal or near-optimal solutions to these problems.

**Problem 1: Eight Queens Puzzle**
The Eight Queens Puzzle involves placing eight queens on an 8x8 chessboard in such a way that no two queens threaten each other. The program employs three local search algorithms: random walk, hill climbing, and simulated annealing; to find solutions to this problem. It then compares their performances to determine which algorithm yields the best results.

**Problem 2: Optimal Route**
In the second problem, the program addresses the task of connecting a collection of points on the plane with straight lines to form a closed figure while minimizing the sum of the lengths of the connecting lines. Similar to the first problem, two local search algorithms, greedy search and simulated annealing, are used to find the optimal arrangement of connections between points. The program compares the results obtained from these algorithms to ascertain which one provides superior solutions.

---

## Algorithms Used

**Random Walk**
- This algorithm randomly selects moves in each iteration without considering whether the move improves the current solution.
- It is useful for exploring the solution space but may not find optimal solutions, especially in complex problems.

**Hill Climbing**
- Hill climbing always moves towards neighboring solutions that improve the current solution.
- It may get trapped in local optima and fail to find global optimal solutions in complex problems.

**Simulated Annealing**
- Simulated annealing is similar to random walk but introduces a probability of accepting worse solutions in certain situations.
- This probabilistic approach allows escaping local optima and exploring different parts of the solution space.

**Greedy Search**
- Greedy search algorithm iteratively selects the best option available at each step without considering the global view of the problem.
- It often leads to locally optimal solutions but may not always produce the globally optimal solution, especially in problems with complex solution spaces.
- Despite its simplicity, greedy search is efficient and suitable for problems where local optimality suffices and computational resources are limited.

---

## Performance Comparison

**Eight Queens Puzzle**
- Random walk typically produces suboptimal solutions due to its random nature.
- Hill climbing tends to get trapped in local optima but performs better than random walk.
- Simulated annealing, with its probabilistic nature, often yields the best solutions by exploring the solution space more effectively.

**Optimal Route**
- Greedy search generally provides the best results but can be sensitive to the order in which the points are defined, occasionally resulting in near-optimal solutions.
- Simulated annealing offers more robust performance and tends to find suboptimal solutions consistently.

---

## Conclusion
- For the Eight Queens Puzzle, simulated annealing emerges as the most effective algorithm due to its ability to explore the solution space effectively and find near-optimal solutions.
- In the case of finding the optimal route among points on the plane, greedy search generally outperforms Simulated Annealing in terms of total distance traveled, although the order of points can affect the results.

---

## Dependencies
- Python 3.x
- NumPy
- Matplotlib

---

By employing local search algorithms, this program demonstrates their effectiveness in solving challenging combinatorial optimization problems and provides insights into their comparative performance.# AI-Optimization-and-Local-Search-Algorithms
