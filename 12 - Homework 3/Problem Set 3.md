# Problem Set 3

## PS3 - Question 1

How many different minimum cuts are there in a tree with n nodes (ie. n - 1 edges) ?

- 2^n - 2
- n
- (n on 2)
- **n - 1**

## PS3 - Question 2

Let "output" denote the cut output by Karger's min cut algorithm on a given connected graph with n vertices, and let p = \frac{1}{n\choose 2}.

Which of the following statements are true?

For hints on this question, you might want to watch the short optional video on "Counting Minimum Cuts".

- **There exists a graph  with  nodes and a min cut  of  such that Pr[out = (A,B)] <= p**
- **For every graph G with n nodes, there exists a min cut (A, B) of G such that Pr[out = (A,B)] >= p**
- **For every graph G with n nodes and every min cut (A, B) of G, Pr[out = (A,B)] >= p**
- For every graph G with n nodes and every min cut (A, B), Pr[out = (A,B)] <=  p
- For every graph G with n nodes, there exists a min cut (A, B) such that Pr[out = (A,B)] <= e p

## PS3 - Question 3

Let 0.5 < a < 1 be some constant. Suppose you are looking for the median element in an array using RANDOMIZED SELECT (as explained in lectures).

What is the probability that after the first iteration the size of the subarray in which the element you are looking for lies is <= alpha times the size of the original array?

- 1 - (alpha/2)
- 1 - alpha
- **2alpha - 1**
- alpha - 1/2

## PS3 - Question 4

Let 0 < a < 1 be a constant, independent of . Consider an execution of RSelect in which you always manage to throw out at least a 1 - alpha fraction of the remaining elements before you recurse.

What is the maximum number of recursive calls you'll make before terminating?

- -\frac{\log(n)}{\alpha}
- -\frac{\log(n)}{\log(1-\alpha)}
- -\frac{\log(n)}{\log(\frac{1}{2}+\alpha)}
- **-\frac{\log(n)}{\log(\alpha)}**

## PS3 - Question 5

The minimum s-t cut problem is the following. The input is an undirected graph, and two distinct vertices of the graph are labelled "s" and "t". The goal is to compute the minimum cut (i.e., fewest number of crossing edges) that satisfies the property that s and t are on different sides of the cut.

Suppose someone gives you a subroutine for this s-t minimum cut problem via an API. Your job is to solve the original minimum cut problem (the one discussed in the lectures), when all you can do is invoke the given min s-t cut subroutine. (That is, the goal is to reduce the min cut problem to the min s-t cut problem.)

Now suppose you are given an instance of the minimum cut problem -- that is, you are given an undirected graph (with no specially labelled vertices) and need to compute the minimum cut.

What is the minimum number of times that you need to call the given min s-t cut subroutine to guarantee that you'll find a min cut of the given graph?

- 2^n
- n
- (n on 2)
- **n -1**
