# Final Exam - Part 1

## Final - Question 1

Recall the Partition subroutine that we used in both QuickSort and RSelect. Suppose that the following array has just been partitioned around some pivot element: 3, 1, 2, 4, 5, 8, 7, 6, 9

Which of these elements could have been the pivot element? (Hint: Check all that apply, there could be more than one possibility!)

- 3
- **5**
- **4**
- 2
- **9**

## Final - Question 2

Here is an array of ten integers: 5 3 8 9 1 7 0 2 6 4

Suppose we run MergeSort on this array. What is the number in the 7th position of the partially sorted array after the outermost two recursive calls have completed (i.e., just before the very last Merge step)? (When we say "7th" position, we're counting positions starting at 1; for example, the input array has a "0" in its 7th position.)

- 1
- 3
- 4
- **2**

## Final - Question 3

What is the asymptotic worst-case running time of MergeSort, as a function of the input array length n??

- \theta(n^2)
- \theta(log n)
- \theta(n)
- **\theta(n log n)**

## Final - Question 4

Consider a directed graph G = (V,E) with non-negative edge lengths and two distinct vertices s and t of V. Let P denote a shortest path from s to t in G. If we add 10 to the length of every edge in the graph, then: [Check all that apply.]

- **If P has only one edge, then P definitely remains a shortest s - t path.**
- **P might or might not remain a shortest s - t path (depending on the graph).**
- P definitely remains a shortest s - t path.
- P definitely does not remain a shortest s -t path.

## Final - Question 5

What is the running time of depth-ﬁrst search, as a function of n and m, if the input graph G = (V,E) is represented by an adjacency matrix (i.e., NOT an adjacency list), where as usual n = |V| and m = |E| ??

- \theta(n*m)
- \theta(n+m)
- \theta(n^2\log m)
- **\theta(n^2)**

## Final - Question 6

What is the asymptotic running time of the Insert and Extract-Min operations, respectively, for a heap with n objects?

- \Theta(n) and \Theta(1)
- \Theta(log n) and \Theta(1)
- \Theta(1) and \Theta(log n)
- **\Theta(log n) and \Theta(log n)**

## Final - Question 7

On adding one extra edge to a directed graph G, the number of strongly connected components...?

- ...cannot decrease by more than 1
- ...cannot decrease
- ...cannot change
- **...might or might not remain the same (depending on the graph).**

## Final - Question 8

What is the asymptotic running time of Randomized QuickSort on arrays of length , in expectation (over the choice of random pivots) and in the worst case, respectively?

- \Theta(n) [expected] and \Theta(n log n) [worst case]
- \Theta(n^2) [expected] and \Theta(n^2) [worst case]
- \Theta(n log n) [expected] and \Theta(n log n) [worst case]
- **\Theta(n log n) [expected] and \Theta(n^2) [worst case]**

## Final - Question 9

Let f and g be two increasing functions, defined on the natural numbers, with f(1),g(1) >= 1. Assume that f(n)=O(g(n)). Is 2^{f(n)}=O(2^{g(n)}) ? (Multiple answers may be correct, check all that apply.)

- **Maybe, maybe not (depends on the functions f and g).**
- **Yes if f(n) <= g(n) for all sufficiently large n**
- Never
- Always

## Final - Question 10

Let  be some constant. Consider running the Partition subroutine on an array with no duplicate elements and with the pivot element chosen uniformly at random (as in QuickSort and RSelect).

What is the probability that, after partitioning, both subarrays (elements to the left of the pivot, and elements to the right of the pivot) have size at least \(\alpha$$ times that of the original array?

- alpha
- 2 - 2alpha
- 1 - alpha
- **1 - 2aplha**

## Final - Question 11

Which of the following statements hold? (As usual n and m denote the number of vertices and edges, respectively, of a graph.) [Check all that apply.]

- **Breadth-first search can be used to compute the connected components of an undirected graph in O(m+n) time.**
- **Breadth-first search can be used to compute shortest paths in O(m+n) time (when every edge has unit length).**
- **Depth-first search can be used to compute the strongly connected components of a directed graph in O(m+n) time.**
- **Depth-first search can be used to compute a topological ordering of a directed acyclic graph in O(m+n) time.**

## Final - Question 12

When does a directed graph have a unique topological ordering?

- **None of the other options.**
- Whenever it is a complete directed graph.
- Whenever it has a unique cycle.
- Whenever it is directed acyclic.

## Final - Question 13

Suppose that a randomized algorithm succeeds (e.g., correctly computes the minimum cut of a graph) with probability p (with 0 < p < 1). Let \epsilon be a small positive number (less than 1).

How many independent times do you need to run the algorithm to ensure that, with probability at least 1 - \epsilon, at least one trial succeeds?

- \frac{\log (p)}{\log \epsilon}
- \frac{\log \epsilon}{\log (p)}
- \frac{\log (1-p)}{\log \epsilon}
- \frac{\log \epsilon}{\log (1-p)}

## Final - Question 14

Suppose you implement the operations Insert and Extract-Min using a sorted array (from biggest to smallest). What is the worst-case running time of Insert and Extract-Min, respectively? (Assume that you have a large enough array to accommodate the Insertions that you face.)

- \Theta(n) and \Theta(n) 
- \Theta(1) and \Theta(n)
- \Theta(log n) and \Theta(1)
- **\Theta(n) and \Theta(1)**

## Final - Question 15

Which of the following patterns in a computer program suggests that a heap data structure could provide a significant speed-up (check all that apply)?

- **Repeated minimum computations**
- Repeated lookups
- **Repeated maximum computations**
- None of the other options

## Final - Question 16

Which of the following patterns in a computer program suggests that a hash table could provide a significant speed-up (check all that apply)?

- None of the other options
- Repeated minimum computations
- Repeated maximum computations
- **Repeated lookups**

## Final - Question 17

Which of the following statements about Dijkstra's shortest-path algorithm are true for input graphs that might have some negative edge lengths? [Check all that apply.]

- **It is guaranteed to terminate.**
- It may or may not terminate (depending on the graph).
- **It may or may not correctly compute shortest-path distances (from a given source vertex to all other vertices), depending on the graph.**

## Final - Question 18

Suppose you are given k sorted arrays, each with n elements, and you want to combine them into a single array of kn elements. Consider the following approach. Divide the k arrays into k/2 pairs of arrays, and use the Merge subroutine taught in the MergeSort lectures to combine each pair. Now you are left with k/2 sorted arrays, each with 2n elements. Repeat this approach until you have a single sorted array with kn elements. What is the running time of this procedure, as a function of k and n?

- \theta(nk\log n)
- \theta(n\log k)
- \theta(nk^2)
- **\theta(nk\log k)**

## Final - Question 19

Running time of Strassen's matrix multiplication algorithm: Suppose that the running time of an algorithm is governed by the recurrence . What's the overall asymptotic running time (i.e., the value of )?

- \theta(n^2)
- \theta(n^{\frac{\log 2}{\log 7}})
- \theta(n^2\log n)
- **\theta(n^{\log_2(7)})**

## Final - Question 20

Recall the Master Method and its three parameters . Which of the following is the best interpretation of , in the context of divide-and-conquer algorithms?

- The rate at which the total work is growing (per level of recursion).
- The rate at which the subproblem size is shrinking (per level of recursion).
- The rate at which the number of subproblems is growing (per level of recursion).
- **The rate at which the work-per-subproblem is shrinking (per level of recursion).**
