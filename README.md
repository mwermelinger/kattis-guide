# A Guide to Kattis Problems

[Kattis](https://open.kattis.com)
is a programming platform with a clean and modern interface.
Problems on Kattis and similar platforms
cover many algorithms and data structures,
and they are good practice to pay attention to details,
separate the wheat from the chaff in a problem description,
and think of edge cases where the algorithm may fail.

Users can register on Kattis with an e-mail or their
Azure, Facebook, Github, Google or LinkedIn accounts.
Users can submit solutions in about 20 different programming languages.
Users solve problems at their leisure but may also participate in time-limited
contests, each with a selection of Kattis problems.

Kattis runs each submission against hidden tests.
If all tests pass, the user gets the points associated with that problem.
Each user's points also contribute to the points of their country and school.
Users, schools and countries are ranked by their points.
Many users don't solve any problem after registering on Kattis.
If you solve just a few easy problems,
you'll climb thousands of places in the rankings.
The [help page](https://open.kattis.com/help) has more details
on how to submit, the possible outcomes, and the scoring system.

Kattis has over 2500 problems from many
[competitions and training sessions](https://open.kattis.com/problem-sources),
so where to start and how to progress?
Kattis suggests problems mostly by difficulty, i.e. number of points.
Here I take some problems from
Steven Halim's [Methods to Solve](https://cpbook.net/methodstosolve) website and classify them according to the algorithmic approach or data structure
I used to solve the problem, which isn't always the one Steven suggests.
I hope this helps you select problems that are appropriate to your knowledge
or your students'.

I aim to list around five problems for each algorithm or data structure,
by order of difficulty, according to my judgement. Your mileage may vary.
Most problems can be listed under two or more categories, depending on the
algorithmic technique(s) and data structure(s) used,
but that would give too much away about how to solve them.

For each problem, I provide a direct link to its Kattis page,
where you can find the number of points and submit your solution.
I also provide the number of lines of code (LOC) of my Python 3 solution,
but longer programs are not necessarily more difficult.
I don't count blank and comment lines, nor
do I use semicolons to join two short lines into one.
I often use list comprehensions and conditional expressions.
The LOC are just a rough indication of how much coding is involved.
Solving Kattis problems is _not_ about playing
[code golf](https://en.wikipedia.org/wiki/Code_golf);
it's about getting the algorithms and data structures right.

- [Input and Output](input.md): read this first;
  it's an overview of the necessary I/O functions
- [Foundations](foundations.md): sequence, selection, iteration,
  integers, floats, strings
- [Ordered collections](ordered.md):
  sorting, lists, stacks, (priority) queues, deques
- [Unordered collections](unordered.md): dictionaries, sets, bags
- [Exhaustive search](exhaustive.md): linear search, backtracking
- [Tree](tree.md): rooted n-ary trees, binary heaps
- [Graph](graph.md): undirected graphs, graph traversals
