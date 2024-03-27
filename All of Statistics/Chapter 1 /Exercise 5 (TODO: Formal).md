## Exercise 5

Suppose we toss a fair coin until we get exactly two heads. Describe the sample space $S$. What is the probability that exactly $k$ tosses are required?

### Solution

Let $C = \lbrace h, t \rbrace$, where $h$ denotes heads and $t$ denotes tails (and $C$ is the set of possible outcomes from our coin). Seeing that we will continue to flip a coin until we achieve exactly two heads, our sample space $S$ will consist of tuples from $C^n$ that contain exactly two instances of $h$. 

Let $A_k \subset S$ symbolise the event where two heads are achieved in exactly $k$ tosses. Informally, we know there are $k \choose 2$ ways to arrange an $k$-tuple with two elements as $h$ and all other elements as $t$. As such $|A_k| = {k \choose 2}$. Simultaneously, given elements of our tuples can only hold one of two values, binary enumeration reveals $|C^k| = 2^k$. Overall, we see that $|A_k|$ out of $|C^k|$ contain exactly two instances of $h$, so

$$P(A_k) = \frac{k \choose 2}{2^k}.$$

*Proof.* Let 

At the very least, we must have $k \ge 2$ with $A_2 = \lbrace (h, h) \rbrace$. In the case $k=2$, we have $C^2 = \lbrac (t,t), (t,h), (h,t), (h,h)$. Given each side is weighted equally and there are four possible outcomes of flipping a coin twice, we have $|C^2| = 4$. Thus,

$$P(A_2) = \frac{|A_2|}{|C^2|} = \frac{k \choose 2}{2^k} = \frac{1}{4}.$$
