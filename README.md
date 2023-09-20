# TravelingSalesPerson
Java implementation of the shortest path algorithm using 3 main approaches: Heuristic, Recursive Backtracking, and Custom approach. Creates a class DGraph to represent a directed graph.
After each algorithm is implemented, they are timed against each other and compared.

# Timings for HEURISTIC:

1st Run: Cost = 3.39, Time = 1 milliseconds

2nd Run: Cost = 3.39, Time = 1 milliseconds

3rd Run: Cost = 3.39, Time = 1 milliseconds

4th Run: Cost = 3.39, Time = 1 milliseconds

5th Run: Cost = 3.39, Time = 1 milliseconds

# Timings for BACKTRACKING:

1st Run: Cost = 1.35, Time = 96 milliseconds

2nd Run: Cost = 1.35, Time = 92 milliseconds

3rd Run: Cost = 1.35, Time = 87 milliseconds

4th Run: Cost = 1.35, Time = 88 milliseconds

5th Run: Cost = 1.35, Time = 94 milliseconds

# Timings for MINE:

1st Run: Cost = 1.67, Time = 23 milliseconds

2nd Run: Cost = 1.67, Time = 22 milliseconds

3rd Run: Cost = 1.67, Time = 24 milliseconds

4th Run: Cost = 1.67, Time = 24 milliseconds

5th Run: Cost = 1.67, Time = 23 milliseconds


# Notes on Algorithms
Heuristic algorithm is currently doing the Nearest-Neighbor approach in which it starts
from city 1 and chooses the closest city to city one. This means its very fast to run,
but it does NOT guarantee the most optimal path.

The Mine approach is a combination of Heuristic and recursion. It chooses its start city
by the one that has the shortest "edge" overall. Then it goes and finds the closest
neighbor and recurses. Instead of trying every single possible combination like backtracking,
it goes through all the nodes (or cities) that are closest to the current city first. Then
it goes through the rest till it finds a solution. So it does not go through every
combination, it just goes through most until it finds a solution by using the closest city.

The Backtracking approach is a brute-force search in which it will try every single
combination (starting from city 1) and records the cost of each path, then it returns
the path with the smallest cost. This Guarantees the MOST optimal path, but it is very
inefficient (runs n!) compared to any other approach.
