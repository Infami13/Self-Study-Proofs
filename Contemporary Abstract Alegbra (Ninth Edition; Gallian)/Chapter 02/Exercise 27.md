# Exercise 27

## Solution

We proceed with induction. Clearly, for our base case, we see $(a^{-1}ba)^1 = a^{-1}ba = a^{-1}b^1a$. Now for our induction step, suppose $(a^{-1}ba)^k = a^{-1}b^ka$ for some natural $k$. We then see 

$$
\begin{align}
(a^{-1}ba)^{k+1} &= (a^{-1}ba)^k(a^{-1}ba) \\
				 &= (a^{-1}b^ka)(a^{-1}ba) \\
				 &= a^{-1}b^kaa^{-1}ba \\
				 &= a^{-1}b^keba \\
				 &= a^{-1}b^kba \\
				 &= a^{-1}b^{k+1}a, \\
\end{align}
$$

where $e$ is the identity element of the group.
