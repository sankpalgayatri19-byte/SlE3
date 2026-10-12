BFS and DFS Graph Search Profiling and Case Analysis System

Project Overview

This project implements Breadth-First Search (BFS) and Depth-First Search (DFS) algorithms to traverse a graph and analyze their execution performance under different test scenarios.

The system evaluates three cases:

- Best Case: Goal node is located at a shallow depth.
- Average Case: Goal node is located at a medium depth.
- Worst Case: Goal node is unreachable.

The project measures execution time and counts expanded nodes to compare the behavior of BFS and DFS.

Objectives

- Implement BFS using a queue ("collections.deque").
- Implement DFS using a stack ("list").
- Compare search performance across different test cases.
- Measure execution time over repeated runs.
- Profile program execution using "py-spy".

Technologies Used

- Python 3
- "collections.deque"
- "time" module
- "py-spy" profiler

Project Structure

IAI_BFS_DFS/
├── script.py
├── README.md
└── AI_CONTRIBUTION_LOG.md

Algorithms

Breadth-First Search (BFS)

BFS explores nodes level by level using a FIFO queue. It uses a visited set to avoid revisiting nodes.

Depth-First Search (DFS)

DFS explores a branch deeply before moving to another branch. It uses a LIFO stack and a visited set.

Test Scenarios

1. Best Case: The goal node is shallow and can be reached quickly.
2. Average Case: The goal node is located at a medium depth.
3. Worst Case: The goal node is unreachable, requiring the algorithm to explore the reachable portion of the graph.

Performance Evaluation

The program measures execution time using Python's "time.time()" function and counts the number of expanded nodes. The documented benchmark uses 100,000 repetitions.

The "py-spy" profiler can be used to sample execution stacks and inspect where the program spends its time.

How to Run

1. Install Python 3.
2. Clone or download the repository.
3. Open a terminal in the project directory.
4. Run:

python script.py

To profile the program with "py-spy", install the profiler and use:

py-spy record -o profile.svg -- python script.py

Note: Profiling commands and outputs depend on your environment and installed tools.

Expected Output

The program should report performance information for BFS and DFS, including execution time and expanded-node counts for the configured test scenarios.

Actual results depend on the graph structure, implementation, and execution environment.

Conclusion

This project demonstrates graph traversal using BFS and DFS, compares their behavior under different goal-node scenarios, and uses execution-time measurements and profiling to study algorithm performance.
