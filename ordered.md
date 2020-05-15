# Ordered collections

These problems can be solved using some form of sequence,
i.e. a collection where the order of items matters.
Some problems become easier by sorting the items.
Sometimes items must be sorted for output, to enable automated testing.

## Sorting

These problems can be solved using function `sorted` or method `sort` to put
the items in ascending or descending order.

- [Cetiri](https://open.kattis.com/problems/cetiri) (7 LOC):
Given 3 integers, find a fourth one to make an arithmetic progression.
Doesn't require loops.

## Stacks

In a stack, the last item to be added is the first to be removed.
Only the last added item can be accessed.
Stacks are useful to process nested items.
In Python, you can use any list as a stack by only using
`a_list.append(...)`, `a_list.pop()`, `len(a_list)` and `a_list[-1]`.

- [Delimiter Soup](https://open.kattis.com/problems/delimitersoup) (17 LOC):
A variation on the classic balanced bracket problem:
report the first wrong closing bracket, if there's one.
