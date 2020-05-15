# Unordered collections

These problems can be solved using unordered collections,
in which the order of items doesn't matter.

## Sets

A set is an unordered collection of unique items, i.e. without duplicates.
Sets are useful if we need:
- efficient removal and addition of items;
- the items that two or more sets have in common;
- the items that are in one set but not the other.

Python has a builtin set type.
If the set has only integers, a list of Booleans may suffice.

- [Booking a Room](https://open.kattis.com/problems/bookingaroom) (5 LOC):
  Given the already booked rooms, and knowing the capacity of the hotel,
  find an available room.

- [Free Food](https://open.kattis.com/problems/freefood) (6 LOC):
  Given several ranges of days, how many days are they in total?

- [Saving Princess Peach](https://open.kattis.com/problems/princesspeach)
  (7 LOC): Which obstacles has Super Mario missed? Requires sorting.

- [CD](https://open.kattis.com/problems/cd) (7 LOC):
  Given two collections of CDs, which are duplicate?
  Due to the number of CDs, requires fast input reading:
  use `stdin.readline()` instead of `input()`.

- [Jolly Jumpers](https://open.kattis.com/problems/jollyjumpers) (17 LOC):
  Given a sequence of integers, do the differences between consecutive integers
  cover all numbers from 1 to n?

## Bags

A bag (or multiset) is an unordered collection with duplicates.
Bags are useful when you need to count the frequency of each item.
Python's class `collections.Counter` provides a bag data structure.

- [Hardwood Species](https://open.kattis.com/problems/hardwoodspecies) (7 LOC):
  Compute the percentage of each tree species in a forest. Requires sorting.

- [Recount](https://open.kattis.com/problems/recount) (6 LOC):
  Check if one candidate has more votes than all the other ones.

- [Zipf's Law](https://open.kattis.com/problems/zipfslaw) (28 LOC):
  Find in a text all words that occur exactly a given number of times.
  Requires string processing.
