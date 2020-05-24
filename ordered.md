# Ordered collections

These problems can be solved using some form of sequence,
i.e. a collection where the order of items matters.

## Lists

Any problem that requires `input().split()` uses a list, but often
it's just to access different parts of the input data.
These problems instead are about processing a list.

1. [Statistics](https://open.kattis.com/problems/statistics) (8 LOC):
See the [Input and Output](input.md) section for details.

## Sorting

Some problems become easier by sorting the items.
Sometimes items must be sorted for output, to enable automated testing.
These problems can be solved using function `sorted` or method `sort` to put
the items in ascending or descending order.

1. [Cetiri](https://open.kattis.com/problems/cetiri) (7 LOC):
Given 3 integers, find a fourth one to make an arithmetic progression.
No loops.

1. [Basic Programming 2](https://open.kattis.com/problems/basicprogramming2)
(43 LOC): Five classic applications of sorting:
find two numbers that add up to a given number; check for duplicates;
check for a majority; find the median; find numbers in a range.

## Stacks

A stack is a last-in-first-out sequence:
only the item last added can be accessed and removed.
<!-- Stacks are useful to process nested items. -->
In Python, a list behaves as a stack if the only operations used are
`a_list.append(...)`, `a_list.pop()`, `len(a_list)` and `a_list[-1]`.

1. [Delimiter Soup](https://open.kattis.com/problems/delimitersoup) (17 LOC):
  A variation on the classic balanced bracket problem:
  report the first wrong closing bracket, if there's one.

1. [Even Up Solitaire](https://open.kattis.com/problems/evenup) (9 LOC):
  Simulate a solitaire game where adjacent cards of even sum are removed.

1. [Backspace](https://open.kattis.com/problems/backspace) (7 LOC):
  Process backspaces in a log of keystrokes to obtain the final text.
  Needs some string processing.

1. [Pairing Socks](https://open.kattis.com/problems/pairingsocks) (13 LOC):
  Try to match pairs of stocks by moving socks from one pile to another.

1. [Game of Throwns](https://open.kattis.com/problems/throwns) (18 LOC):
  A variation of the classic use of stacks to undo previous commands.
