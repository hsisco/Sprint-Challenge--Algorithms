#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a) Because the algorithm asks to simply add n^2 to itself until it reaches a certain level, which will increase the time as n increases, the runtime of this loop is O(n).

b) The outer loop iterates through each i until it reaches n, which would be O(n) on its own. The inner loop doubles 1 until it's greater than n, which would be O(log2 n). These nested loops leave us with an O(n log n) runtime.

c) By running a constant equation over _bunnies_ recursively, this has a linear O(n) runtime.

## Exercise II

We can assume that:
- each floor is an element in an array of floors
- we must compare each floor to see if a broken egg is either true or false

To do this, we have to find the floor mid-way up the building and see if that produces a true or false on a broken egg. If true, we move down to the bottom 25% and try again, or if false, we move up to the top 75%. We repeat until we find the highest floor that returns a false broken egg, which would be _f_. Because we are constantly halving the testing field, the runtime is O(log n).