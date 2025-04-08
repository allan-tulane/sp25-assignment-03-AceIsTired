# CMPS 2200 Assignment 3
## Answers

**Name:** Jamari Ross


Place all written answers from `assignment-03.md` here for easier grading.

**1.) Making Change**
**a.** Start with the largest $2^k$ that is $\leq N.$ Subtract this value from N, and log how many coins of that value were used. Then, move on to the next value $2^k$ that is $\leq N$, and repeat the steps until $N = 0$, then return your list of coins used.

**b.** The greedy choice at each step guarentees the maximum is being used each time. After subtracting the coin value at each level, we are left witht he equation $N - 2^k$, which is the same as the original problem wth a smaller value. This is also the optimal solution since it is solving smaller subproblems.

**c.** The work and span of this algorithm is $O(log n)$.

---------------
**2.) Making Change Again**
**a.** A counterexample for this algorithm would be if we had $D = {1, 5, 6}$ and the value we want to reach, $N$, is = 10. Using our previous strategy, we would get:
+ $10 - 6 = 4$
+ $4 - 1 = 3$
+ $3 - 1 = 2$
+ $2 - 1 = 1$
+ $1 - 1 = 0$

Which gets us 5 coins. This is not optimal, as you could simply subtract two 5 value coins and end up with a total number of 2 coins compared to 5.

**b.** To find the best answer for N, we format the problem into smaller subsections for each denomination of size $N - Di$. If we know the solution to a smaller problem, we can use that same soluition to make the answer for N, by adding another coin. This leaves us with the optimal solution.

**c.** The work and span is $O(n)$.

---------------
**3.) Edit Distance**
**a.** DONE

**b.** I tried a bunch of things but could not get it to work.