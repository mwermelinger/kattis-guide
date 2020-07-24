# Exhaustive search

These problems can be solved by exhaustively generating candidate solutions and
keeping those that satisfy the problem's requirements, e.g. the best solution.
The search may stop early, e.g. if only the first solution is needed.
This approach is also called brute-force search, or generate and test.

## Linear search

In a linear search, the candidates are the items in a given collection:
list, string, set, etc.
Candidates are 'generated' by iterating through the collection.
The search may require an additional data structure to
keep information about the items already processed.

1. [Hot Hike](https://open.kattis.com/problems/hothike) (10 LOC):
   Given the air temperatures over several days,
   find the lowest n that minimises the temperature on days n and n+2.

1. [Pea Soup and Pancakes](https://open.kattis.com/problems/peasoup) (15 LOC):
   Given a list of restaurants and their menus,
   find the first one that serves pea soup and pancakes.

1. [Saving Princess Peach](https://open.kattis.com/problems/princesspeach)
   (7 LOC): Find all obstacles that Super Mario missed.

1. [ICPC Awards](https://open.kattis.com/problems/icpcawards) (8 LOC):
   Given a list of university teams, find the first team of each university.

1. [Amalgamated Artichokes](https://open.kattis.com/problems/artichoke)
   (11 LOC): Given the fluctuation of stock prices over time,
   find the start and end of the biggest price drop.
   Use the `math` library functions `sin` and `cos` to compute the prices.

## Combinations

In these problems, each candidate is a combination of digits, letters or
other items. Generating all combinations may require nested loops.

1. [Heir's Dilemma](https://open.kattis.com/problems/heirsdilemma) (14 LOC):
   Count how many 6-digit PINs, within a given range,
   have distinct digits and are divisible by each of their digits.
