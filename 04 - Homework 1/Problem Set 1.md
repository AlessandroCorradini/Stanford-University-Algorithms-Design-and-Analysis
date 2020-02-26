# Problem Set 1

## PS1 - Question 1

3-way-Merge Sort : Suppose that instead of dividing in half at each step of Merge Sort, you divide into thirds, sort each third, and finally combine all of them using a three-way merge subroutine. What is the overall asymptotic running time of this algorithm? (Hint: Note that the merge step can still be implemented in O(n) time.)

- n
- n^2 log(n)
- n(log(n))^2
- **n log(n)**

## PS1 - Question 2

You are given functions f and g such that f(n)=O(g(n)). Is f(n)*log_2(f(n)^c) = O(g(n)*log_2(g(n))) ? (Here c is some positive constant.) You should assume that  and  are nondecreasing and always bigger than 1.

- Sometimes yes, sometimes no, depending on the functions f and g
- False
- Sometimes yes, sometimes no, depending on the constant c
- **True**

## PS1 - Question 3

Assume again two (positive) nondecreasing functions f and g such that f(n)=O(g(n)). Is 2^{f(n)}=O(2^{g(n)}) ? (Multiple answers may be correct, you should check all of those that apply.)

- **Yes if f(n) <= le g(n) for all sufficiently large**
- **Sometimes**
- Never
- Always

## PS1 - Question 4

k-way-Merge Sort. Suppose you are given k sorted arrays, each with kn elements, and you want to combine them into a single array of  elements. Consider the following approach. Using the merge subroutine taught in lecture, you merge the first 2 arrays, then merge the 3rd given array with this merged version of the first two arrays, then merge the 4th given array with the merged version of the first three arrays, and so on until you merge in the final (k^(th)) input array. What is the running time taken by this successive merging algorithm, as a function of k and n? (Optional: can you think of a faster way to do the k-way merge procedure ?)

- \theta(n^2k)
- \theta(nk)
- \theta(n \log(k))
- \theta(nk^2)

## PS1 - Question 5

Arrange the following functions in increasing order of growth rate (with  following  in your list if and only if ).

a) 2^{2^n}
b) 2^{n^2}
c) n^2\log(n)
d) n
e) n^{2^n}

Write your 5-letter answer, i.e., the sequence in lower case letters in the space provided. For example, if you feel that the answer is a->b->c->d->e (from smallest to largest), then type abcde in the space provided without any spaces in between the string.

You can assume that all logarithms are base 2 (though it actually doesn't matter).

**dcbae**

## Optional Theory Problems

1. You are given as input an unsorted array of n distinct numbers, where n is a power of 2. Give an algorithm that identifies the second-largest number in the array, and that uses at most  comparisons.

2. You are a given a unimodal array of n distinct elements, meaning that its entries are in increasing order up until its maximum element, after which its elements are in decreasing order. Give an algorithm to compute the maximum element that runs in O(log n) time.

3. You are given a sorted (from smallest to largest) array A of n distinct integers which can be positive, negative, or zero. You want to decide whether or not there is an index i such that A[i] = i. Design the fastest algorithm that you can for solving this problem.
