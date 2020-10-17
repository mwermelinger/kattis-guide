# Input / Output

Each Kattis problem requires data to be read from the standard input, and
the results to be written to the standard output. There are different ways
to do so in Python, depending on the problem. Most Kattis problems fall into one
of the following categories. I give one example per category.

## No input

Without input, all you need is the `print()` function to write to standard
output.

- [Hello World!](https://open.kattis.com/problems/hello) (1 LOC):
The classic first program. It doesn't get easier than this, and yet over
[40% of the submissions failed](https://open.kattis.com/problems/hello/statistics)!
A sobering reminder than even the most trivial problem demands
attention to details and checking before submitting.

## One datum per line, fixed lines

Problems in this category have a fixed number of lines, given in the problem
description, and each line has a single datum, e.g. one number.

To read a single line from the standard input, use `input()`, which returns a
string. If a string represents a number, use function `int()` or `float()` to
convert it to an integer or floating-point number.

For example, if the problem consists of reading 3 floats from the input, one per line, and produce the smallest of them, the solution would be:
```py
print(min(float(input()), float(input()), float(input())))
```

- [Simple Addition](https://open.kattis.com/problems/simpleaddition) (1 LOC):
Add two large integers. Trivial in Python.

## Multiple data per line, fixed lines

In this category, the number of input lines is fixed but some lines may
contain more than one number or string, usually separated by spaces.

For these problems, use the string method `split()` to separate the input line
into a list of strings. If the data is separated by anything other than spaces,
give the separator (e.g. `','`) as an argument to `split()`.

For example, if the input is a single line of space-separated integers and the
output is the sum of those integers, one solution is:

```py
total = 0
for number in input().split():
    total += int(number)
print(total)
```
With comprehensions, a one-line solution is:
```py
print(sum(int(number) for number in input().split()))
```

- [Solving for Carrots](https://open.kattis.com/problems/carrots) (1 LOC):
A silly description of a trivial problem that makes
an excellent introduction to ignoring irrelevant details.

## _n_ lines

These problems have a variable number _n_ of lines, but _n_ is given at the
start of the input, and so the lines can be read with a for-loop.

Consider the sum example again, but this time, each integer is on its line, and the first line is the number of lines that follow.
The solution becomes:
```py
total = 0
for _ in range(int(input())):   # I use name _ if the variable isn't needed
    total += int(input())
print(total)
```

- [Help a PhD candidate out!](https://open.kattis.com/problems/helpaphd)
(3 LOC): A silly problem, but good to practice the input techniques so far.
My 3-line solution uses a particular Python function.
The problem can be solved without it.

## End marker

These problems have a variable number of lines, and their number is unknown at
the start. Instead, there is a marker signalling the end of input.
Processing such inputs requires a repeat-until loop, using a `while` statement.

Imagine the sum example has one integer per line and the last integer is zero.
The solution becomes:
```py
total = 0
number = int(input())
while number != 0:
    total += number
    number = int(input())
print(total)
```

- [Left Beehind](https://open.kattis.com/problems/leftbeehind) (11 LOC):
Make a decision based on two integers.
The input has two integers per line, terminating with two zeros.

## End of file

In these problems, there's no extra information at the start or end of the input.
If each test case consists of a single line, the most straightforward approach is to loop
over each line of the standard input, which is `sys.stdin`.

Returning to the example, if the input is one integer per line
and all integers are to be added, the solution becomes:
```py
from sys import stdin

total = 0
for line in stdin:
    total += int(line)
print(total)
```
or:
```py
from sys import stdin

print(sum(int(line) for line in stdin))
```

- [A Different Problem](https://open.kattis.com/problems/different) (4 LOC):
Compute the difference between a pair of numbers, with one pair per line.
<!--
The `input()` function returns a string without a newline at the end, but
the lines obtained by iterating over `stdin` do include a newline.
The newline character is removed or ignored by `split()`, `int()` and `float()`,
but for some problems you may need to remove it explicitly with the `rstrip()`
method, which removes all whitespace from the right end of a string.
 -->

## Formatted output
Some problems require the output to be formatted in a particular way,
e.g. without a space between values, or with a certain number of digits after the decimal point.

If spaces do not separate output items, you can use `print(..., end='')` or
string concatenation. However, often the easiest way to cope with much of output
formatting is to use Python's f-strings.

- [Statistics](https://open.kattis.com/problems/statistics) (8 LOC):
Compute the maximum, minimum and range of the given values.
One test case per line. Write the case number to the output.

## Fast I/O

Some problems have long inputs or long outputs.
You may get a 'Time Limit Exceeded' error. In those cases,
use `stdin.readline()` instead of `input()`
and `stdout.write()` instead of `print()`.

The `readline()` function returns the empty string on the end of input.

The `write()` function takes a string to be written as-is.
You must write all spaces and newlines yourself,
and convert data to strings using the function `str()`.

Here's the last example again:
```py
from sys import stdin, stdout

total = 0
line = stdin.readline()
while line:                 # same as while line != '':
    total += int(line)
    line = stdin.readline()
stdout.write(str(total))
stdout.write('\n')
```

- [CD](https://open.kattis.com/problems/cd) (7 LOC):
  Given two collections of CDs, which are duplicate?
