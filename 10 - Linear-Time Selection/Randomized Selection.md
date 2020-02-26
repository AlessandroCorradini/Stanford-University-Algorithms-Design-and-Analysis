# Randomized Selection

## Q1

Suppose we are looking for the 5th order statistic in an input array of length 10. We partition the array, and the pivot winds up in the third position of the partitioned array.

On which side of the pivot do we recurse, and what order statistic should we look for?

- The 3rd order statistic on the left side of the pivot.
- **The 2nd order statistic on the right side of the pivot.**
- The 5th order statistic on the right side of the pivot.
- "Not enough information to answer question" – we might need to recurse on the left or the right side of the pivot.

## Q2

What is the running time of the RSelect algorithm if pivots are always chosen in the worst possible way?

- theta(n)
- theta(n log n)
- theta(n^2)
- theta(2^n)
