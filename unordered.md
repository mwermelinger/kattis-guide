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
