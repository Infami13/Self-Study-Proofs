Let $P(W), P(M), P(L)$ denote the probability a computer owner uses Windows, Macintosh, and Linux respectively. As such,

$$
\begin{align}
P(W) &= 0.5 \\
P(M) &= 0.3 \\
P(L) &= 0.2. \\
\end{align}
$$

Let $P(V)$ denote the probability an owner has a computer virus. From the information provided, we also know

$$
\begin{align}
P(V | W) &= 0.82 \\
P(V | M) &= 0.65 \\
P(V | L) &= 0.5. \\
\end{align}
$$

Utilizing Bayes' Theorem (analogous to Example 1.19), we find

$$
\begin{align}
P(W|V) &= \frac{P(V|W)P(W)}{P(V|W)P(W) + P(V|M)P(M) + P(V|L)P(L)} \\
       &= \frac{0.82 \cdot 0.5}{0.82 \cdot 0.5 + 0.65 \cdot 0.3 + 0.5 \cdot 0.2} \\
       &\approx 0.58156.
\end{align}
$$
