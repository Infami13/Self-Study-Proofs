# Exercise 13

## Lemma

For elements $a$ and $x$ in a group, we have $(xax^{-1})^n = xa^nx^{-1}$ for each natural $n$.

*Proof*. We proceed with induction. Clearly, for our base case, we see $(xax^{-1})^1 = xax^{-1} = xa^1x^{-1}$. Now for our induction step, suppose $(xax^{-1})^k = xa^kx^{-1}$ for some natural $k$. We then see 

$$
\begin{align}
(xax^{-1})^{k+1} &= (xax^{-1})^k(xax^{-1}) \\
				 &= (xa^kx^{-1})(xax^{-1}) \\
				 &= xa^kx^{-1}xax^{-1} \\
				 &= xa^keax^{-1} \\
				 &= xa^kax^{-1} \\
				 &= xa^{k+1}x^{-1}, \\
\end{align}
$$

where $e$ is the identity element of the group.

## Solution

In the case $|a|$ is finite, say $|a| = n$ for some natural $n$, we know from our lemma that $(xax^{-1})^n = xa^nx^{-1}$. Simplifying this further, we have $xa^nx^{-1} = xex^{-1} = xx^{-1} = e$, where $e$ is the identity element of the group. That is to say, $|xax^{-1}| \le n = |a|$. To show that $|xax^{-1}| \ge |a|$, suppose to the contrary that there is some non-zero natural $m < n$ such that $(xax^{-1})^m = e$. Then $xa^mx^{-1} = e$, which implies $a^m = x^{-1}x = e$. However, this contradicts $|a| = n$, so $|xax^{-1}| \ge |a|$. All together, $|xax^{-1}| = |a|$.

In the case $|a|$ is infinite, suppose to the contrary that $|xax^{-1}| = n$ for some finite $n$. From our lemma again, we see that $(xax^{-1})^n = xa^nx^{-1}$. Given the order of $xax^{-1}$, we know $xa^nx^{-1} = e$. Multiplying the left by $x^{-1}$ and the right by $x$, we see

$$
\begin{align}
x^{-1}xa^nx^{-1}x &= x^{-1}ex \\
ea^ne &= x^{-1}x \\
a^n &= e. \\
\end{align}
$$

However, this contradicts the idea that $a$ has infinite order. Thus, $xax^{-1}$ has infinite order as well.
