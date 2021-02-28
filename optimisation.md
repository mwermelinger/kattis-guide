# Optimisation

Optimisation problems ask for the best solution,
according to some criterion for what's best.
[Search algorithms](exhaustive.md) can also solve optimisation problems.

## Greedy algorithms

A greedy algorithm constructs the solution incrementally,
at each step choosing the best of the available alternatives.
For example, if the solution is a collection of items, a greedy algorithm will
start with an empty collection and keep adding the best available item
until obtaining a complete solution.
Greedy algorithms often involve sorting the alternatives from best to worst.

Many optimisation problems can't be solved by greedy algorithms,
because the best solution isn't necessarily made of locally best choices.
For example, always going to the nearest place from the current one doesn't
always lead to the shortest path from one place to another.

1. [Minimum Scalar Product](https://open.kattis.com/problems/minimumscalar)
   (6 LOC): Given two sequences of integers x and y of the same length n,
   rearrange each sequence so that the sum x[1]·y[1] + ... + x[n]·y[n]
   is the smallest possible.
