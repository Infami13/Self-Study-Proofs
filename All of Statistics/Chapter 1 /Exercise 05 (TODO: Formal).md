## Exercise 5

Suppose we toss a fair coin until we get exactly two heads. Describe the sample space $S$. What is the probability that exactly $k$ tosses are required?

### Solution

Let $C = \lbrace h, t \rbrace$, where $h$ denotes heads and $t$ denotes tails (and $C$ is the set of possible outcomes from our coin). 

Using an informal approach, seeing that we will continue to flip a coin until we achieve exactly two heads, our sample space $S$ will consist of ordered tuples from $\bigcup\nolimits_{n=2}^\infty C^n$ that contain exactly two instances of $h$. Let $A_k \subset S$ symbolise the event where two heads are achieved in exactly $k$ tosses. We know each tuple in $A_k$ has $h$ as its last element (we stop flipping once we achieve the second head). The other $h$ must occupy one of the remaining $k - 1$ spaces, with all other elements being $t$. So, $|A_k| = {k - 1 \choose 1} = k-1$. Simultaneously, given elements of our tuples can only hold one of two values, binary enumeration reveals $|C^k| = 2^k$. That is, the number of possible outcomes from exactly $k$ tosses is $2^k$. Overall, we see that $|A_k|=k-1$ out of $|C^k|=2^k$ tuples (of $k$ length) contain exactly two instances of $h$ with $h$ as the last element. So


$$P(A_k) = \frac{k - 1}{2^k}.$$

*Proof.* Let 

At the very least, we must have $k \ge 2$ with $A_2 = \lbrace (h, h) \rbrace$. In the case $k=2$, we have $C^2 = \lbrac (t,t), (t,h), (h,t), (h,h)$. Given each side is weighted equally and there are four possible outcomes of flipping a coin twice, we have $|C^2| = 4$. Thus,

$$P(A_2) = \frac{|A_2|}{|C^2|} = \frac{k \choose 2}{2^k} = \frac{1}{4}.$$
