# Foundations

These problems don't use any complicated algorithms or data structures.
They help get used to the submission system and the various forms of input.
As mentioned in the introduction, within each category,
problems are listed from easiest to less easy, in my opinion of course.

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

## Selection

These problems can be solved with if-statements alone. No loops required.

1. [Moscow Dream](https://open.kattis.com/problems/moscowdream) (5 LOC):
  Check that four integers satisfy some conditions.

1. [Wizard of Odds](https://open.kattis.com/problems/wizardofodds) (5 LOC):
  Check that two integers satisfy a condition.

1. [Judging Moose](https://open.kattis.com/problems/judgingmoose) (7 LOC):
  Describe the antlers of a moose.

1. [Eating Out](https://open.kattis.com/problems/eatingout) (3 LOC):
  Check if people in a restaurant, each choosing a certain number of dishes,
  may end up not choosing the same dish. A problem that is
  easy to code but requires some thinking to get the formula.

## Iteration

These problems require a for- or while-loop because either
the input contains multiple lines, or the problem itself requires a loop.

1. [R2](https://open.kattis.com/problems/r2) (3 LOC):
Given the average of two integers and one of them, find the other one.
The input has 2 integers per line, until the end of file.

1. [A Different Problem](https://open.kattis.com/problems/different) (4 LOC):
See the [Input and Output](input.md) section for details.
Doesn't require if-statements.

1. [Left Beehind](https://open.kattis.com/problems/leftbeehind) (11 LOC):
See the [Input and Output](input.md) section for details.

1. [Thanos](https://open.kattis.com/problems/thanos) (7 LOC):
Simulate population growth and find out in which year resources aren't enough.
The first line is the number of test cases, one per line.
A nice simple problem that uses a for-loop (to process all test cases)
and a while-loop (to solve each test case).

1. [Tarifa](https://open.kattis.com/problems/tarifa) (6 LOC):
Given the allowance on a data plan, and given the past monthly consumption,
how much data is available this month? Unused data carries forward.
The input is a single test case. The second line is the number of past months,
followed by the consumption in each month, one per line.

<!-- - [Roaming Romans](https://open.kattis.com/problems/romans) (5 LOC): -->

## Floats

These problems involve floating-point numbers, some of
which can be tricky due to precision and rounding issues.
<!--
Function `float` converts a string to a floating-point number.
Function [`round`](https://docs.python.org/3/library/functions.html#round)
changes the precision of a floating-point number or converts it to an integer.
-->

1. [Pizza Crust](https://open.kattis.com/problems/pizza2) (2 LOC):
  What percentage of a pizza has cheese, knowing the width of the crust?
  No if-statements or loops.

1. [Euler's Number](https://open.kattis.com/problems/eulersnumber) (6 LOC):
  Approximate Euler's number through a series of factorials.
  Doesn't require mathematical knowledge. Just implement the given formula.

1. [Roaming Romans](https://open.kattis.com/problems/romans) (5 LOC):
  Convert English miles to Roman paces.
  Requires some care because Python rounds floats to the nearest even integer, not necessarily up.

1. [Herman](https://open.kattis.com/problems/herman) (4 LOC):
  What is the area of a circle in normal and in Manhattan/taxi geometry?
  Use `math.pi` for the former. Draw on grid paper to see the latter.
  No if-statements or loops.

## Strings

Almost every problem requires printing a string as part of the output.
These problems however require some string processing: comparing strings,
substring matching with the `in` operator, formatting the output, etc.

1. [IsItHalloween.com](https://open.kattis.com/problems/isithalloween) (2 LOC):
  Check if input is one of two dates. No loops required.

1. [Help a PhD candidate out!](https://open.kattis.com/problems/helpaphd)
(3 LOC): See the [Input and Output](input.md) section for details.

1. [Drinking Song](https://open.kattis.com/problems/drinkingsong) (12 LOC):
  Print out the '99 bottles of beer' song for any drink and number of bottles.
  The text varies when there's one or no bottle left.
