# Ordered collections

These problems can be solved using some form of sequence,
i.e. a collection where the order of items matters.

## Lists

Any problem that requires `input().split()` uses a list, but often
it's just to access different parts of the input data.
These problems instead are about processing a list.

1. [Statistics](https://open.kattis.com/problems/statistics) (8 LOC):
   See the [Input and Output](input.md) section for details.

1. [Backspace](https://open.kattis.com/problems/backspace) (7 LOC):
   Process backspaces in a log of keystrokes to obtain the final text.
   Needs some string processing.

1. [Basic Programming 1](https://open.kattis.com/problems/basicprogramming1)
   (35 LOC): Seven small problems on integer lists, most of them trivial.

1. [Integer Lists](https://open.kattis.com/problems/integerlists) (24 LOC):
   Reverse a list and/or remove its first item several times.
   Print the resulting list. Needs string processing.

## Sorting

Some problems become easier by sorting the items.
Sometimes items must be sorted for output, to enable automated testing.
These problems can be solved using function `sorted` or method `sort` to put
the items in ascending or descending order.

1. [Line Them Up](https://open.kattis.com/problems/lineup) (9 LOC):
   Detect if a sequence is in ascending order, descending order or neither.

1. [Cetiri](https://open.kattis.com/problems/cetiri) (7 LOC):
   Given 3 integers, find a fourth one to make an arithmetic progression.
   No loops needed.

1. [Bus Numbers](https://open.kattis.com/problems/busnumbers) (18 LOC):
   Print a list of numbers (e.g. 143 142 141) in a compact way (e.g. 141-143).

1. [Basic Programming 2](https://open.kattis.com/problems/basicprogramming2)
   (43 LOC): Five classic applications of sorting:
   find two numbers that add up to a given number; check for duplicates;
   check for a majority; find the median; find numbers in a range.

## Stacks

A stack is a last-in-first-out sequence:
only the item last added can be accessed and removed.
Stacks are useful to process nested items.

In Python, a list behaves as a stack if the only operations used are
`a_list.append(...)`, `a_list.pop()`, `len(a_list)` and `a_list[-1]`.

1. [Delimiter Soup](https://open.kattis.com/problems/delimitersoup) (17 LOC):
   A variation on the classic balanced bracket problem:
   report the first wrong closing bracket, if there's one.

1. [Even Up Solitaire](https://open.kattis.com/problems/evenup) (9 LOC):
   Simulate a solitaire game where adjacent cards of even sum are removed.

1. [Pairing Socks](https://open.kattis.com/problems/pairingsocks) (13 LOC):
   Try to match pairs of stocks by moving socks from one pile to another.

1. [Game of Throwns](https://open.kattis.com/problems/throwns) (18 LOC):
   A variation of the classic use of stacks to undo previous commands.

1. [I Can Guess the Data Structure!](https://open.kattis.com/problems/guessthedatastructure) (30 LOC): see below.

## Priority queues

A priority queue maintains items ordered by priority, which is typically given
by an integer, but could be any ordered values.
In a min-priority queue the lowest value represents the highest priority;
in a max-priority queue the highest value represents the highest priority.
Python's module `heapq` implements a min-priority queue with a binary heap.

Some of these problems may be solved with two priority queues.

1. [I Can Guess the Data Structure!](https://open.kattis.com/problems/guessthedatastructure) (30 LOC):
   From the observed behaviour of a black-box data structure, infer if
   it's a stack, queue, priority queue or neither of them.

1. [Knigs of the Forest](https://open.kattis.com/problems/knigsoftheforest)
   (21 LOC): Each year, a tournament is won by the strongest candidate.
   The winner is replaced by a newcomer the next year. Knowing the strength of
   a candidate and the year he joins the tournament, in which year will he win?

1. [Continuous Median](https://open.kattis.com/problems/continuousmedian)
   (22 LOC): Re-compute the median every time an integer is added.
   Output the sum of all medians.

1. [Jane Eyre](https://open.kattis.com/problems/janeeyre) (22 LOC):
   Anna reads books in alphabetical order of their title. Given her list of
   unread books (including _Jane Eyre_) and the time it takes to read each,
   and given a list of when further books will be added to the unread pile,
   when will Anna finish reading _Jane Eyre_?

1. [Stock Prices](https://open.kattis.com/problems/stockprices) (30 LOC):
   Simulate stock market deals to determine the current stock price.
