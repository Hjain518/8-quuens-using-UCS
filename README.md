# 8 Queens Problem using Uniform Cost Search(UCS)

UCS is just a variant of Dijikstra's Algorithm.
Instead of inserting all vertices into a priority queue, we insert only source.
UCS is useful for infinite graphs and those graph which are too large to represent in the memory, mainly used in Artificial Intelligence.

# Problem
The eight queens problem is the problem of placing eight queens on an 8×8 chessboard such that none of them attack one another (no two are in the same row, column, or diagonal).

## Implementation
We use priority queue for UCS with path cost of all the children = 1(i.e all the paths have equal chances of being choosen).

We keep placing queen column wise each in every row and proceed further for next row until the problem condition is satisfied or not and when we reach the last row and for any column in the last row if we can successfully place the last queen then we print that solution and exit, otherwise repeat this process until we get any single correct placement of 8 queens.
