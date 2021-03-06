# Trees

Trees are used to represent hierarchical information or to organise data to speed up searches.

<!-- One node is the root of the tree. Each node has zero or more children nodes.
In an _n_-ary tree, each node has at most _n_ children.
A leaf is a childless node.
 -->

## Paths

- [Kitten on a Tree](https://open.kattis.com/problems/kitten) (11 LOC):
  Print the path from a given node to the root.

## Binary Heap

A binary heap is a complete binary tree where each node's value is smaller
(or larger, in a max-heap) than its children's values.
Binary heaps are used to implement priority queues because
they can be efficiently stored and manipulated as an array (Python list).

These problems require knowing how binary heap nodes are indexed,
in particular how to go from a node to its left or right child, and vice-versa.

1. [A Rational Sequence (Take 3)](https://open.kattis.com/problems/rationalsequence3) (9 LOC):
   Consider a binary tree where each node is systematically labelled with a
   fraction. What is the fraction in the n-th node? Use recursion.

1. [A Rational Sequence 2](https://open.kattis.com/problems/rationalsequence2) (13 LOC):
   The inverse of the previous problem: given a fraction, in which node is it?

1. [Numbers On a Tree](https://open.kattis.com/problems/numbertree) (12 LOC):
   Consider a complete binary tree with nodes numbered right to left,
   from the right-most leaf upwards to the root.
   Given a path from the root to a node, what's the number of that node?
   The input is just one line, but it may have one or two data.
