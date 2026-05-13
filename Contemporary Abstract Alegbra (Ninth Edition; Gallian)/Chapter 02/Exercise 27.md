# Exercise 27

## Solution

For convenience, let $e$ represent the identity element of the group.

In the case $n = 0$, we see immediately that $(a^{-1}ba)^0 = e = a^{-1}a = a^{-1}ea = a^{-1}b^0a$.

In the case $n > 0$, we proceed with induction. Clearly, for our base case, we see $(a^{-1}ba)^1 = a^{-1}ba = a^{-1}b^1a$. Now for our induction step, suppose $(a^{-1}ba)^k = a^{-1}b^ka$ for some natural $k$. We then see 

$$
\begin{align}
(a^{-1}ba)^{k+1} &= (a^{-1}ba)^k(a^{-1}ba) \\
				 &= (a^{-1}b^ka)(a^{-1}ba) \\
				 &= a^{-1}b^kaa^{-1}ba \\
				 &= a^{-1}b^keba \\
				 &= a^{-1}b^kba \\
				 &= a^{-1}b^{k+1}a. \\
\end{align}
$$

Lastly, in the case $n < 0$, we take $(a^{-1}ba)^n(a^{-1}ba)^{-n} = e$. From our previous case, we know that $(a^{-1}ba)^{-n} = a^{-1}b^{-n}a$ given $-n > 0$. Through algebraic manipulation, we find

$$
\begin{align}
(a^{-1}ba)^n(a^{-1}b^{-n}a) &= e \\
(a^{-1}ba)^na^{-1}b^{-n}a &= e \\
(a^{-1}ba)^na^{-1}b^{-n}aa^{-1} &= ea^{-1} \\
(a^{-1}ba)^na^{-1}b^{-n}e &= a^{-1} \\
(a^{-1}ba)^na^{-1}b^{-n} &= a^{-1} \\
(a^{-1}ba)^na^{-1}b^{-n}b^n &= a^{-1}b^n \\
(a^{-1}ba)^na^{-1}e &= a^{-1}b^n \\
(a^{-1}ba)^na^{-1} &= a^{-1}b^n \\
(a^{-1}ba)^na^{-1}a &= a^{-1}b^na \\
(a^{-1}ba)^ne &= a^{-1}b^na \\
(a^{-1}ba)^n &= a^{-1}b^na. \\
\end{align}
$$
