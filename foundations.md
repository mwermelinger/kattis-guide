# Foundations

These are among the simplest Kattis problems.
They are a good way to get used to the submission system and the
various forms of input.

Many users don't solve any problem after registering on Kattis.
If you solve just one of these problems
you'll climb thousands of places in the rankings.

## Sequence

These problems can be solved without any if-statements or loops.
You may need to use `abs`, `min` or `max` to avoid if-statements.

- [Hello World!](https://open.kattis.com/problems/hello) (1 LOC):
The classic 'Hello world' program.
No input; just one line of output, using `print`.
It doesn't get easier than this, and yet over
[40% of the submissions](https://open.kattis.com/problems/hello/statistics)
failed! A sobering reminder than even the most trivial problem demands
attention to details and checking before submitting.

- [Simple Addition](https://open.kattis.com/problems/simpleaddition) (1 LOC):
Add two large integers. Trivial in Python.
Use `int(input())` to read each integer.

- [Solving for Carrots](https://open.kattis.com/problems/carrots) (1 LOC):
A silly description of a trivial problem.
A good introduction to ignoring irrelevant details.
The input is a single line with 2 integers.
Use `input().split()` to separate them into a list.

- [Faktor](https://open.kattis.com/problems/faktor) (2 LOC):
A little arithmetic tongue-in-cheek problem about the academic obsession with
bibliometrics. The problem description explains the necessary concepts.


## Selection

These problems can be solved with if-statements alone. No loops required.

- [Moscow Dream](https://open.kattis.com/problems/moscowdream) (5 LOC):
  Check that four integers satisfy some conditions.

- [Wizard of Odds](https://open.kattis.com/problems/wizardofodds) (5 LOC):
  Check that two integers satisfy a condition.

- [Judging Moose](https://open.kattis.com/problems/judgingmoose) (7 LOC):
  Describe the antlers of a moose.

- [Eating Out](https://open.kattis.com/problems/eatingout) (3 LOC):
  Check if people in a restaurant, each choosing a certain number of dishes,
  may end up not choosing the same dish. A typical example of a problem that is
  easy to code but requires some thinking to get the formula.


## Iteration

These problems require a for- or while-loop because either
the input contains multiple test cases, or the problem itself requires a loop.

Kattis problems with multiple test cases tend to fall into these categories:
- the input terminates at the end of the file;
- the input terminates with a special marker;
- the first line states how many test cases there are.


- [R2](https://open.kattis.com/problems/r2) (3 LOC):
Given the average of two integers and one of them, find the other one.
The input has 2 integers per line.
Use `for line in sys.stdin:` to process all lines.

- [Left Beehind](https://open.kattis.com/problems/leftbeehind) (11 LOC):
Make a decision based on 2 integers.
The input has two integers per line, terminating with two zeros.
To process all lines, use the same approach as for the previous problem or
write a repeat-until loop with `while`.

- [Thanos](https://open.kattis.com/problems/thanos) (7 LOC):
Simulate population growth and find out in which year resources aren't enough.
The first line is the number of test cases, one per line.
A nice simple problem that uses a for-loop (to process all test cases)
and a while-loop (to solve each test case).

- [Tarifa](https://open.kattis.com/problems/tarifa) (6 LOC):
Given the allowance on a data plan, and given the past monthly consumption,
how much data is available this month? Unused data carries forward.
The input is a single test case. The second line is the number of past months,
followed by the consumption in each month, one per line.

<!-- - [Roaming Romans](https://open.kattis.com/problems/romans) (5 LOC): -->

## Floats

These problems involve floating-point numbers,
which can be tricky due to precision and rounding issues.
Function `float` converts a string to a floating-point number.
Function [`round`](https://docs.python.org/3/library/functions.html#round)
changes the precision of a floating-point number or converts it to an integer.

- [Roaming Romans](https://open.kattis.com/problems/romans) (5 LOC):
  Convert English miles to Roman paces.
  Requires some care because Python rounds floats to the nearest even integer, not necessarily up.

## Strings

Almost every problem requires printing a string as part of the output.
These problems however require some string processing: comparing strings,
substring matching with the `in` operator, etc.
In some problems, the output items are not separated by spaces:
use `print(..., end='')` or f-strings.

- [IsItHalloween.com](https://open.kattis.com/problems/isithalloween) (2 LOC):
  Check if input is one of two dates. No loops required.

- [Drinking Song](https://open.kattis.com/problems/drinkingsong) (12 LOC):
  Print out the '99 bottles of beer' song for any drink and number of bottles.
  The text varies when there's one or no bottle left.
