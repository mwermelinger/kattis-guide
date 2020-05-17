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

- [Basic Programming 2](https://open.kattis.com/problems/basicprogramming2)
  (43 LOC): Five classic applications of sorting:
  find two numbers that add up to a given number, check for duplicates,
  check for a majority, find the median, find numbers in a range.

## Stacks

A stack is a last-in-first-out sequence:
only the item last added can be accessed and removed.
<!-- Stacks are useful to process nested items. -->
In Python, a list behaves as a stack if only using
`a_list.append(...)`, `a_list.pop()`, `len(a_list)` and `a_list[-1]`.

- [Delimiter Soup](https://open.kattis.com/problems/delimitersoup) (17 LOC):
  A variation on the classic balanced bracket problem:
  report the first wrong closing bracket, if there's one.

- [Even Up Solitaire](https://open.kattis.com/problems/evenup) (9 LOC):
  Simulate a solitaire game where adjacent cards of even sum are removed.

- [Backspace](https://open.kattis.com/problems/backspace) (7 LOC):
  Process backspaces in a log of keystrokes to obtain the final text.
  Needs some string processing.

- [Pairing Socks](https://open.kattis.com/problems/pairingsocks) (13 LOC):
  Try to match pairs of stocks by moving socks from one pile to another.

- [Game of Throwns](https://open.kattis.com/problems/throwns) (18 LOC):
  A variation of the classic use of stacks to undo previous commands.
