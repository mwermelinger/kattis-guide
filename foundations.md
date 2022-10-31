# Foundations

These problems don't require any data structure or complicated algorithm.
They help get used to the submission system and the various forms of input.
As mentioned in the introduction, within each category,
problems are listed from easiest to not so easy, in my opinion.

## Sequence

These problems can be solved without any if-statements or loops.
You may need to use `abs`, `min` or `max` to avoid if-statements.

1. [Hello World!](https://open.kattis.com/problems/hello) (1 LOC):
   See the [Input and Output](input.md) section for details.

1. [Simple Addition](https://open.kattis.com/problems/simpleaddition) (1 LOC):
   See the [Input and Output](input.md) section for details.

1. [Solving for Carrots](https://open.kattis.com/problems/carrots) (1 LOC):
   See the [Input and Output](input.md) section for details.

1. [Faktor](https://open.kattis.com/problems/faktor) (2 LOC):
   A little arithmetic tongue-in-cheek problem about the academic obsession with
   bibliometrics. The problem description explains the necessary concepts.

1. [Planina](https://open.kattis.com/problems/planina) (1 LOC):
   Compute the number of points on a grid, after _n_ iterations of a given
   procedure to create points. Once the formula has been derived,
   the code is trivial, using the power operator `**`.

## Selection

These problems can be solved with if-statements alone. No loops required.

1. [Quadrant Selection](https://open.kattis.com/problems/quadrant) (6 LOC):
   Given the x and y coordinates of a point, print in which quadrant it is.

1. [Moscow Dream](https://open.kattis.com/problems/moscowdream) (5 LOC):
   Check that four integers satisfy some conditions.

1. [Wizard of Odds](https://open.kattis.com/problems/wizardofodds) (5 LOC):
   Check that two integers satisfy a condition.

1. [Judging Moose](https://open.kattis.com/problems/judgingmoose) (7 LOC):
   Describe the antlers of a moose.

1. [Eating Out](https://open.kattis.com/problems/eatingout) (3 LOC):
   Check if people in a restaurant, each choosing a certain number of dishes,
   may end up not choosing the same dish.
   Easy to code, but requires some thinking to get the formula.
   
1. [R2](https://open.kattis.com/problems/r2) (3 LOC):
   Given the average of two integers and one of them, find the other one.

## Iteration

These problems require a for- or while-loop because either
the input contains multiple lines, or the problem itself requires a loop.

1. [A Different Problem](https://open.kattis.com/problems/different) (4 LOC):
   See the [Input and Output](input.md) section for details.
   Doesn't require if-statements.

1. [Left Beehind](https://open.kattis.com/problems/leftbeehind) (11 LOC):
   See the [Input and Output](input.md) section for details.

1. [Thanos](https://open.kattis.com/problems/thanos) (7 LOC):
   Simulate the growth of a population and find out in which year
   the resources aren't enough.
   <!-- The first line is the number of test cases, one per line. -->
   A nice simple problem that uses a for-loop to process all test cases,
   and a while-loop to solve each test case.

1. [Tarifa](https://open.kattis.com/problems/tarifa) (6 LOC):
   Given the allowance on a data plan and the past monthly consumption,
   how much data is available this month? Unused data carries forward.
   <!-- The input is a single test case.
   The second line is the number of past months,
   followed by the consumption in each month, one per line. -->

## Floats

These problems involve floating-point numbers, some of
which can be tricky due to precision and rounding issues.
You may need the `math` library for some of the problems.
<!--
Function `float` converts a string to a floating-point number.
Function [`round`](https://docs.python.org/3/library/functions.html#round)
changes the precision of a floating-point number or converts it to an integer.
-->

1. [A Real Challenge](https://open.kattis.com/problems/areal) (3 LOC):
   Given the area of a square pasture, how long is the fence?
   No if-statements or loops.

1. [Pizza Crust](https://open.kattis.com/problems/pizza2) (2 LOC):
   What percentage of a pizza has cheese, knowing the width of the crust?
   No if-statements or loops.

1. [Euler's Number](https://open.kattis.com/problems/eulersnumber) (6 LOC):
   Approximate Euler's number through a series of factorials.
   This problem doesn't require mathematical knowledge:
   just translate the given formula to code.

1. [Roaming Romans](https://open.kattis.com/problems/romans) (5 LOC):
   Convert English miles to Roman paces. No loops. Requires some care
   because Python rounds floats to the nearest even integer, not necessarily up.

1. [Herman](https://open.kattis.com/problems/herman) (4 LOC):
   What is the area of a circle in normal and in Manhattan/taxi geometry?
   Draw on grid paper to see the latter. No if-statements or loops.

## Strings

Almost every problem requires printing a string as part of the output,
but these problems require some string processing: comparing strings,
matching substrings with the `in` operator,
calculating the length with the `len` function, formatting the output, etc.

1. [IsItHalloween.com](https://open.kattis.com/problems/isithalloween) (2 LOC):
   Check if the input is one of two dates. No loops required.

1. [Avion](https://open.kattis.com/problems/avion) (7 LOC):
   Report which given strings have a particular substring.

1. [Cryptographer's Conundrum](https://open.kattis.com/problems/conundrum)
   (4 LOC): Given a string, count how many letters must be replaced
   to obtain another string.

1. [Help a PhD candidate out!](https://open.kattis.com/problems/helpaphd)
   (3 LOC): See the [Input and Output](input.md) section for details.

1. [Drinking Song](https://open.kattis.com/problems/drinkingsong) (12 LOC):
   Print out the '99 bottles of beer' song for any drink and number of bottles.
   The text varies when there's one or no bottle left.
