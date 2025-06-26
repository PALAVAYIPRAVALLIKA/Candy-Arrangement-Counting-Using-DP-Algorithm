# Candy Sampler Combinations – Dynamic Programming Approach
This project calculates the number of ways to form candy samplers of a given size using square and long candies. It applies dynamic programming to efficiently solve the combinatorial problem with configurable candy types and sizes.
## Problem Statement
Given:
A sampler of size n
s varieties of square candies (occupy 1 unit of space)
l varieties of long candies (occupy 2 units of space)
Determine the number of different ways to completely fill the sampler.
## Approach
The problem is solved using dynamic programming by breaking it into smaller subproblems and building up solutions iteratively.
Problem Decomposition

A square candy reduces the sampler size by 1 → dp[i-1] × s
A long candy reduces the sampler size by 2 → dp[i-2] × l

 Recurrence Relation
dp[i] = dp[i-1] × s + dp[i-2] × l;
Where:
dp[i] = number of ways to fill a sampler of size i;
s = number of square candy types;
l = number of long candy types
## Base Cases
dp[0] = 1       # One way to make a sampler of size 0 (empty)
dp[1] = s       # Only square candies can be used
## Time and Space Complexity
| Complexity Type  | Value  | Explanation                                |
| ---------------- | ------ | ------------------------------------------ |
| Time Complexity  | `O(n)` | Each value from 1 to n is computed once    |
| Space Complexity | `O(n)` | Due to storage of all intermediate results |
| Space Optimized  | `O(1)` | Only last 2 values needed for computation  |
##  Technologies Used

- Python  
- Dynamic Programming  
- Git & GitHub  

