# Unordered collections

These problems can be solved with collections
in which the order of items doesn't matter.

## Dictionaries

A dictionary (or hash table) is an unordered collection of key-value pairs
with unique keys. Dictionaries allow quick access to a value by key.
Dictionaries are useful to map one collection of items to another.

Python has a built-in dictionary type.
If the keys are integers from a known range, a list may suffice,
with the indices being the keys.

1. [Relocation](https://open.kattis.com/problems/relocation) (8 LOC):
Keep track of companies relocating to a different number on the same street
and determine the distance (number of doors) between any two companies.

1. [Preludes](https://open.kattis.com/problems/chopin) (15 LOC):
Print the alternate name for a musical key, e.g. Gb major -> F# major.
The problem description explains all you need to know.

1. [Linden Mayor System](https://open.kattis.com/problems/lindenmayorsystem)
(9 LOC):  A simple simulation of a computational biology system, the
[L-system](https://en.wikipedia.org/wiki/L-system).
The problem description explains all you need to know. Needs string processing.

1. [Metaprogramming](https://open.kattis.com/problems/metaprogramming)
(24 LOC):  An interpreter for simple integer comparisons.
Requires some string processing.

## Sets

A set is an unordered collection of unique items, i.e. without duplicates.
Sets are useful if we need:
- efficient removal and addition of items;
- the items that two or more sets have in common;
- the items that are in one set but not the other.

Python has a builtin set type.
If the set has only integers, a list of Booleans may suffice.

1. [Booking a Room](https://open.kattis.com/problems/bookingaroom) (5 LOC):
Given the already booked rooms, and knowing the capacity of the hotel,
find an available room.

1. [Free Food](https://open.kattis.com/problems/freefood) (6 LOC):
Given several ranges of days, how many days are there in total?

1. [Quick Brown Fox](https://open.kattis.com/problems/quickbrownfox) (8 LOC):
   Find all English letters that don't occur in the given text.

1. [CD](https://open.kattis.com/problems/cd) (7 LOC):
See the [Input and Output](input.md) section for details.

1. [Jolly Jumpers](https://open.kattis.com/problems/jollyjumpers) (17 LOC):
Given a sequence of integers, do the differences between consecutive integers
cover all numbers from 1 to n?

## Bags

A bag (or multiset) is an unordered collection with duplicates.
Bags are useful when you need to count the frequency of each item.
Python's class `collections.Counter` provides a bag data structure.

1. [Hardwood Species](https://open.kattis.com/problems/hardwoodspecies) (6 LOC):
  Compute the percentage of each tree species in a forest. Requires sorting.

1. [Recount](https://open.kattis.com/problems/recount) (6 LOC):
  Check if one candidate has more votes than all the other ones.

1. [Peragrams](https://open.kattis.com/problems/peragrams) (10 LOC):
  What is the least number of characters we must remove from a given string to
  obtain an anagram (i.e. a rearrangement) of a palindrome (a string that is
      the same forwards and backwards)? No string processing required.

1. [Zipf's Law](https://open.kattis.com/problems/zipfslaw) (28 LOC):
  Find in a text all words that occur exactly a given number of times.
  Requires string processing.
