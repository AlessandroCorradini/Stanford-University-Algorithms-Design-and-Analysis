# Problem Set 6

## PS6 - Question 1

Suppose we use a hash function h to hash n distinct keys into an array T of length m. Assuming simple uniform hashing --- that is, with each key mapped independently and uniformly to a random bucket --- what is the expected number of keys that get mapped to the first bucket? More precisely, what is the expected cardinality of the set \{k:h(k)=1\}.

- 1/m
- 1/n
- m/(2n)
- n/(2m)
- m/n
- **n/m**

## PS6 - Question 2

You are given a binary tree (via a pointer to its root) with  nodes, which may or may not be a binary search tree. How much time is necessary and sufficient to check whether or not the tree satisfies the search tree property?

- \Theta(height)
- \Theta(log n)
- \Theta(n log n)
- **\Theta(n)**

## PS6 - Question 3

You are given a binary tree (via a pointer to its root) with n nodes. As in lecture, let size(x) denote the number of nodes in the subtree rooted at the node x.

How much time is necessary and sufficient to compute size(x) for every node x of the tree?

- \Theta(height)
- \Theta(n^2)
- \Theta(n log n)
- **\Theta(n)**

## PS6 - Question 4

Which of the following is not a property that you expect a well-designed hash function to have?

- The hash function should "spread out" most (i.e., "non-pathological") data sets (across the buckets/slots of the hash table).
- The hash function should be easy to compute (constant time or close to it).
- The hash function should be easy to store (constant space or close to it).
- **The hash function should "spread out" every data set (across the buckets/slots of the hash table).**

## PS6 - Question 5

Suppose we relax the third invariant of red-black trees to the property that there are no three reds in a row. That is, if a node and its parent are both red, then both of its children must be black. Call these relaxed red-black trees.

Which of the following statements is not true?

- The height of every relaxed red-black tree with n nodes is O(log n).
- Every red-black tree is also a relaxed red-black tree.
- There is a relaxed red-black tree that is not also a red-black tree.
- **Every binary search tree can be turned into a relaxed red-black tree (via some coloring of the nodes as black or red).**