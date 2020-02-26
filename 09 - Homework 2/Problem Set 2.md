# Problem Set 2

## PS2 - Question 1

Note: If you take this quiz multiple times, you may see different variations of this question.

This question will give you further practice with the Master Method. Suppose the running time of an algorithm is governed by the recurrence T(n) = 9*T(n/3) + n^2.

What's the overall asymptotic running time (i.e., the value of T(n))?

- \theta(n^{3.17})
- \theta(n^2)
- \theta(n log n)
- **\theta(n^2 log n)**

## PS2 - Question 2

Consider the following pseudocode for calculating  (where a and b are positive integers)

FastPower(a,b) :

if b = 1

return a

else

c := a*a

ans := FastPower(c,[b/2])

if b is odd

return a*ans

else return ans

end

Here [x] denotes the floor function, that is, the largest integer less than or equal to x.

Now assuming that you use a calculator that supports multiplication and division (i.e., you can do multiplications and divisions in constant time), what would be the overall asymptotic running time of the above algorithm (as a function of b)?

- \Theta(b log(b))
- \Theta(b)
- \Theta(sqrt(b))
- **\Theta(log(b))**

## PS2 - Question 3

Let 0 < alpha < 0.5 be some constant (independent of the input array length n). Recall the Partition subroutine employed by the QuickSort algorithm, as explained in lecture.

What is the probability that, with a randomly chosen pivot element, the Partition subroutine produces a split in which the size of the smaller of the two subarrays is >= alpha times the size of the original array?

- 2 - 2alpha
- alpha
- 1 - alpha
- **1 - 2aplha**

## PS2 - Question 4

Now assume that you achieve the approximately balanced splits above in every recursive call --- that is, assume that whenever a recursive call is given an array of length k, then each of its two recursive calls is passed a subarray with length between alphak and (1 - alpha)k (where alpha is a fixed constant strictly between 0 and 0.5).

How many recursive calls can occur before you hit the base case? Equivalently, which levels of the recursion tree can contain leaves?

Express your answer as a range of possible numbers d, from the minimum to the maximum number of recursive calls that might be needed.

- -\frac{\log(n)}{\log(1-2*\alpha)} \le d \le -\frac{\log(n)}{\log(1-\alpha)}
- 0 \le d \le -\frac{\log(n)}{\log(\alpha)}
- -\frac{\log(n)}{\log(1-\alpha)} \le d \le -\frac{\log(n)}{\log(\alpha)}
- **-\frac{\log(n)}{\log(\alpha)} \le d \le -\frac{\log(n)}{\log(1-\alpha)}**

## PS2 - Question 5

Define the recursion depth of QuickSort to be the maximum number of successive recursive calls before it hits the base case --- equivalently, the number of the last level of the corresponding recursion tree. Note that the recursion depth is a random variable, which depends on which pivots get chosen.

What is the minimum-possible and maximum-possible recursion depth of QuickSort, respectively?

- **Minimum: \Theta(log(n)) ; Maximum: O(n)**
- Minimum:  \Theta(log(n)); Maximum: \Theta(n log(n))
- Minimum: O(1) ; Maximum: O(n)
- Minimum: O(sqrt(n)) ; Maximum: O(n)
