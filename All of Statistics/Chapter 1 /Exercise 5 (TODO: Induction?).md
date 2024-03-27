## Exercise 5

Suppose we toss a fair coin until we get exactly two heads. Describe the sample space $S$. What is the probability that exactly $k$ tosses are required?

### Solution

Let $C = \lbrace h, t \rbrace$, where $h$ denotes heads and $t$ denotes tails (and $C$ is the set of possible outcomes from our coin). Seeing that we will continue to flip a coin until we achieve exactly two heads, our sample space $S$ will consist of order pairs from $C^n$ that contain exactly two instances of $h$. 

Let $A_k \subset S$ symbolise the event where two heads are achieved in exactly $k$ tosses. At the very least, we must have $k \ge 2$ with $A_2 = \lbrace (h, h) \rbrace$. Given each side is weighted equally and there are four possible outcomes of flipping a coin twice, we have $|C^2| = 4$. Thus,

$$P(A_2) = \frac{|A_2|}{|C^2|} = \frac{k \choose 2}{2^k} = \frac{1}{4}.$$
