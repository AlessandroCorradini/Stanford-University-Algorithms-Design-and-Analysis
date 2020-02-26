# Final Exam - Part II

## Final - Question 1

Consider a connected undirected graph with distinct edge costs. Which of the following are true? [Check all that apply.]

- **Suppose the edge e is the cheapest edge that crosses the cut (A,B). Then e belongs to every minimum spanning tree.**
- **Suppose the edge e is the most expensive edge contained in the cycle C. Then e does not belong to any minimum spanning tree.**
- Suppose the edge e is not the cheapest edge that crosses the cut (A,B). Then e does not belong to any minimum spanning tree.
- **The minimum spanneing tree is unique.**

## Final - Question 2

You are given a connected undirected graph G with distinct edge costs, in adjacency list representation. You are also given the edges of a minimum spanning tree T of G. This question asks how quickly you can recompute the MST if we change the cost of a single edge. Which of the following are true? [RECALL: It is not known how to deterministically compute an MST from scratch in O(m) time, where m is the number of edges of G.] [Check all that apply.]

- **Suppose e \in T and we decrease the cost of e. Then, the new MST can be recomputed in O(m) deterministic time.**
- **Suppose e \notin T and we increase the cost of e. Then, the new MST can be recomputed in O(m) deterministic time.**
- **Suppose e \in T and we increase the cost of e. Then, the new MST can be recomputed in O(m) deterministic time.**
- **Suppose e \notin T and we decrease the cost of e. Then, the new MST can be recomputed in O(m) deterministic time.**

## Final - Question 3

Which of the following problems reduce, in a straightforward way, to the minimum spanning tree problem? [Check all that apply.]

- **The minimum bottleneck spanning tree problem. That is, among all spanning trees of a connected graph with edge costs, compute one with the minimum-possible maximum edge cost.**
- **Given a connected undirected graph G = (V, E) with positive edge costs, compute a minimum-cost set F \subseteq E such that the graph (V,E-F) is acyclic.**
- The single-source shortest-path problem.
- **The maximum-cost spanning tree problem. That is, among all spanning trees of a connected graph with edge costs, compute one with the maximum-possible sum of edge costs.**

## Final - Question 4

Which of the following graph algorithms can be implemented, using suitable data structures, in O(m log n) time? (As usual, m and n denote the number of edges and vertices, respectively.) [Check all that apply.]

- The Bellman-Ford shortest-path algorithm.
- **Prim's minimum spanning tree algorithm.**
- Johnson's all-pairs shortest-path algorithm.
- **Kruskal's minimum spanning tree algorithm.**

## Final - Question 5

Recall the greedy clustering algorithm from lecture and the max-spacing objective function. Which of the following are true? [Check all that apply.]

- **If the greedy algorithm produces a k-clustering with spacing S, then every other k-clustering has spacing at most S.**
- Suppose the greedy algorithm produces a k-clustering with spacing S. Then, if x, y are two points in a common cluster of this k-clustering, the distance between x and y is at most S.
- This greedy clustering algorithm can be viewed as Prim's minimum spanning tree algorithm, stopped early.
- **If the greedy algorithm produces a k-clustering with spacing S, then the distance between every pair of points chosen by the greedy algorithm (one pair per iteration) is at most S.**

## Final - Question 6

We are given as input a set of n jobs, where job j has a processing time p_j and a deadline d_j. Recall the definition of completion times C_j from the video lectures. Given a schedule (i.e., an ordering of the jobs), we define the lateness l_j of job j as the amount of time C_j = d_j after its deadline that the job completes, or as 0 if C_j <= d_j.

Our goal is to minimize the total lateness,

\sum_{j} l_j

Which of the following greedy rules produces an ordering that minimizes the total lateness?

You can assume that all processing times and deadlines are distinct.

WARNING: This is similar to but not identical to a problem from Problem Set #1 (the objective function is different).

- Schedule the requests in increasing order of the product d_j * p_j
- Schedule the requests in increasing order of deadline d_j
- Schedule the requests in increasing order of processing time p_j
- **None of the other options are correct**

## Final - Question 7

Consider an alphabet with five letters,{a, b, c, d, e}, and suppose we know the frequencies f_a = 0.28, f_b = 0.27, f_c = 0.2, f_d = 0.15, and f_e = 0.1. What is the expected number of bits used by Huffman's coding scheme to encode a 1000-letter document?

- 2450
- 2230
- 2520
- **2250**

## Final - Question 8

Of the following dynamic programming algorithms covered in lecture, which ones always perform O(1) work per subproblem? [Check all that apply.]

- The dynamic programming algorithm for the optimal binary search tree problem.
- **The dynamic programming algorithm for the sequence alignment problem.**
- The Bellman-Ford shortest-path algorithm.
- **The dynamic programming algorithm for the knapsack problem.**
- **The Floyd-Warshall all-pairs shortest-paths algorithm.**

## Final - Question 9

Which of the following statements are true about the tractability of the Knapsack problem? [Check all that apply.]

- **Assume that P != NP. The special case of the Knapsack problem in which all item values are positive integers less than or equal to n^5, where n is the number of items, can be solved in polynomial time.**
- **If there is a polynomial-time algorithm for the Knapsack problem in general, then P=NP.**
- Assume that P != NP. The special case of the Knapsack problem in which all item values, item sizes, and the knapsack capacity are positive integers, can be solved in polynomial time.
- **Assume that P != NP. The special case of the Knapsack problem in which all item sizes are positive integers less than or equal to n^5, where n is the number of items, can be solved in polynomial time.**

## Final - Question 10

Assume that P != NP. Which of the following extensions of the Knapsack problem can be solved in time polynomial in n, the number of items, and M, the largest number that appears in the input? [Check all that apply.]

- You are given n items with positive integer values and sizes, as usual, and m positive integer capacities, W_1, W_2, ..., W_m . These denote the capacities of different Knapsacks, where m could be as large as \Theta(n). The problem is to pack items into these knapsacks to maximize the total value of the packed items. You are not allowed to split a single item between two of the knapsacks.
- **You are given  items with positive integer values and sizes, as usual, and two positive integer capacities, W_1 and W_2. The problem is to pack items into these two knapsacks (of capacities W_1 and W_2) to maximize the total value of the packed items. You are not allowed to split a single item between the two knapsacks.**
- **You are given  items with positive integer values and sizes, and a positive integer capacity W, as usual. The problem is to compute the max-value set of items with total size exactly W. If no such set exists, the algorithm should correctly detect that fact.**
- **You are given n items with positive integer values and sizes, and a positive integer capacity W, as usual. You are also given a budget k <= n on the number of items that you can use in a feasible solution. The problem is to compute the max-value set of at most k items with total size at most W.**

## Final - Question 11

Assume that P != NP. The following problems all take as input two strings X and Y, of length m and n, over some alphabet \Sigma. Which of them can be solved in O(mn) time? [Check all that apply.]

- **Consider the following variation of sequence alignment. Instead of a single gap penalty alpha_gap, you're given two numbers a and b. The penalty of inserting k gaps in a row is now defined as ak + b, rather than k * alpha_gap. Other penalties (for matching two non-gaps) are defined as before. The goal is to compute the minimum-possible penalty of an alignment under this new cost model.**
- **Compute the length of a longest common subsequence of X and Y. (Recall a subsequence need not be consecutive. For example, the longest common subsequence of "abcdef" and "afebcd" is "abcd".)**
- **Assume that X and Y have the same length . Does there exist a permutation f, mapping each i \in \{1,2,\ldots,n\} to a distinct f(i) \in \{1,2,\ldots,n\}, such that X_i = Y_{f(i)} for every i = 1, 2, ..., n?**
- **Compute the length of a longest common substring of X and Y. (A substring is a consecutive subsequence of a string. So "bcd" is a substring of "abcdef", whereas "bdf" is not.)**

## Final - Question 12

Assume that P != NP. Which of the following problems can be solved in polynomial time? [Check all that apply.]

- **Given a directed graph with nonnegative edge lengths, compute the length of a maximum-length shortest path between any pair of vertices (i.e., \max_{u,v \in V} d(u,v), where d(u,v) is the shortest-path distance between u and v).**
- Given a directed graph with nonnegative edge lengths, compute the length of a longest cycle-free path between any pair of vertices (i.e.\max_{u,v \in V} \max_{P \in \mathcal{P}_{uv}} \sum_{e \in P} c_e, where P_uv denotes the set of cycle-free u-v paths).
- Given a directed graph with real-valued edge lengths, compute the length of a longest cycle-free path between any pair of vertices (i.e., \max_{u,v \in V} \max_{P \in \mathcal{P}_{uv}} \sum_{e \in P} c_e, where P_uv denotes the set of cycle-free u-v paths).
- **Given a directed acyclic graph with real-valued edge lengths, compute the length of a longest path between any pair of vertices.**

## Final - Question 13

Recall the all-pairs shortest-paths problem. Which of the following algorithms are guaranteed to be correct on instances with negative edge lengths that don't have any negative-cost cycles? [Check all that apply.]

- **Run the Bellman-Ford algorithm  times, once for each choice of a source vertex.**
- Run Dijkstra's algorithm  times, once for each choice of a source vertex.
- The Floyd-Warshall algorithm.
- **Johnson's reweighting algorithm.**

## Final - Question 14

Consider an instance of the optimal binary search tree problem with 7 keys (say 1,2,3,4,5,6,7 in sorted order) and frequencies w_1 = 0.2, w_2 = 0.05, w_3 = 0.17, w_4 = 0.1, w_5 = 0.2, w_6 = 0.03, w_7 = 0.25. What is the minimum-possible average search time of a binary search tree with these keys?

- 2.33
- 2.18
- 2.29
- **2.23**

## Final - Question 15

Suppose a computational problem \Pi that you care about is NP-complete. Which of the following are true? [Check all that apply.]

- Since the dynamic programming algorithm design paradigm is only useful for designing exact algorithms, there's no point in trying to apply it to the problem \Pi.
- **If your boss criticizes you for failing to find a polynomial-time algorithm for \Pi, you can legitimately claim that thousands of other scientists (including Turing Award winners, etc.) have likewise tried and failed to solve \Pi.**
- NP-completeness is a "death sentence"; you should not even try to solve the instances of \Pi that are relevant for your application.
- **You should not try to design an algorithm that is guaranteed to solve \Pi correctly and in polynomial time for every possible instance (unless you're explicitly trying to prove that P = NP).**

## Final - Question 16

Which of the following statements are logically consistent with our current state of knowledge (i.e., with the mathematical statements that have been formally proved)? [Check all that apply.]

- **There is an NP-complete problem that is polynomial-time solvable.**
- **There is no NP-complete problem that can be solved in O(n^{\log n}) time, where n is the size of the input.**
- Some NP-complete problems are polynomial-time solvable, and some NP-complete problems are not polynomial-time solvable.
- **There is an NP-complete problem that can be solved in O(n^{\log n}) time, where n is the size of the input.**

## Final - Question 17

Of the following problems, which can be solved in polynomial time by directly applying algorithmic ideas that were discussed in lecture and/or the homeworks? [Check all that apply.]

- **Given an undirected graph G and a constant value for  (i.e., k = O(1), independent of the size of G), does G have a vertex cover of size at most k?**
- **Given an undirected graph G and a value for k such that k = \Theta(\log n), where  is the number of vertices of G, does G have a vertex cover of size at most k?**
- **Given an undirected graph G and a constant value for k (i.e., k = O(1), independent of the size of G), does G have an independent set of size at least k?**
- Given an undirected graph G and a value for k such that k = \Theta(\log n), where n is the number of vertices of G, does G have an independent set of size at least k?

## Final - Question 18

In lecture we gave a dynamic programming algorithm for the traveling salesman problem. Does this algorithm imply that P=NP? [Check all that apply.]

- No. A polynomial-time algorithm for the traveling salesman problem does not necessarily imply that P=NP.
- No. Since we perform a super-polynomial amount of work extracting the final TSP solution from the solutions of all of the subproblems, the algorithm does not run in polynomial time.
- Yes, it does.
- **No. Since there are an exponential number of subproblems in our dynamic programming formulation, the algorithm does not run in polynomial time.**
- No. Since we sometimes perform a super-polynomial amount of work computing the solution of a single subprolem, the algorithm does not run in polynomial time.

## Final - Question 19

Consider the Knapsack problem and the following greedy algorithm: (1) sort the items in nonincreasing order of value over size (i.e., the ratio v_i/w_i); (2) return the maximal prefix of items that fits in the Knapsack (i.e., the k items with the largest ratios, where k is as large as possible subject to the sum of the item sizes being at most the knapsack capacity W ). Which of the following are true? [Check all that apply.]

- **If all items have the same size, then this algorithm always outputs an optimal solution (no matter how ties are broken).**
- **If the size of every item is at most 20% of the Knapsack capacity (i.e., w_i \le W/5 for every i), then this algorithm is guaranteed to output a feasible solution with total value at least 80% times that of an optimal solution.**
- If all items have the same value/size ratio, then this algorithm always outputs an optimal solution (no matter how ties are broken).
- **If all items have the same value, then this algorithm always outputs an optimal solution (no matter how ties are broken).**
- This algorithm always outputs a feasible solution with total value at least 50% times that of an optimal solution.

## Final - Question 20

Which of the following statements are true about the generic local search algorithm? [Check all that apply.]

- The generic local search algorithm is guaranteed to terminate in a polynomial number of iterations.
- **The output of the generic local search algorithm generally depends on the choice of the starting point.**
- **The output of the generic local search algorithm generally depends on the choice of the superior neighboring solution to move to next (in an iteration where there are multiple such solutions).**
- The generic local search algorithm is guaranteed to eventually converge to an optimal solution.