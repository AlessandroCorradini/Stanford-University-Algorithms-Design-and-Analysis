# Problem Set 5

## PS5 - Question 1

Consider a directed graph with distinct and nonnegative edge lengths and a source vertex s. Fix a destination vertex t, and assume that the graph contains at least one s-t path.

Which of the following statements are true? Check all that apply.

- **The shortest (i.e., minimum-length) s-t path might have as many as n - 1 edges, where n is the number of vertices.**
- **There is a shortest s-t path with no repeated vertices (i.e., a "simple" or "loopless" such path).**
- The shortest s-t path must include the minimum-length edge of G.
- The shortest s-t path must exclude the maximum-length edge of G.

## PS5 - Question 2

Consider a directed graph G = (V, E) and a source vertex s with the following properties: edges that leave the source vertex s have arbitrary (possibly negative) lengths; all other edge lengths are nonnegative; and there are no edges from any other vertex to the source s.

Does Dijkstra's shortest-path algorithm correctly compute shortest-path distances (from ) in this graph?

- Only if we add the assumption that G contains no directed cycles with negative total weight. incorrect
- Never
- Maybe, maybe not (depends on the graph)
- **Always**

## PS5 - Question 3

Suppose you implement the functionality of a priority queue using a sorted array (e.g., from biggest to smallest).

What is the worst-case running time of Insert and Extract-Min, respectively? (Assume that you have a large enough array to accommodate the Insertions that you face.)

- \Theta(n) and \Theta(n)
- \Theta(1) and \Theta(n)
- \Theta(log n) and \Theta(1)
- **\Theta(n) and \Theta(1)**

## PS5 - Question 4

Suppose you implement the functionality of a priority queue using an unsorted array.

What is the worst-case running time of Insert and Extract-Min, respectively? (Assume that you have a large enough array to accommodate the Insertions that you face.)

- \Theta(n) and \Theta(n)
- \Theta(n) and \Theta(n)
- \Theta(n) and \Theta(n)
- **\Theta(n) and \Theta(n)**

## PS5 - Question 5

You are given a heap with  elements that supports Insert and Extract-Min.

Which of the following tasks can you achieve in O(log n) time?

- None of these.
- Find the largest element stored in the heap.
- Find the median of the elements stored in the heap.
- **Find the fifth-smallest element stored in the heap.**
