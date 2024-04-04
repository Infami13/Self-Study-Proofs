## Exercise
For any group elements $a$ and $b$, prove that $|ab| = |ba|$.

### Lemma
Let $G$ be a group with $a, b\in G$. Then, $b(ab)^n = (ba)^n b$.

*Proof.* We will prove our lemma using induction. For the base case $n = 1$, we have 
$$b(ab)^n = b(ab)^1 = bab = (ba)^1b = (ba)^nb.$$

For the induction step, assume $b(ab)^n = (ba)^n b$ holds true for positive integer $n$. Then

$$\begin{align}
b(ab)^{n+1} &= b(ab)^n(ab) \\
&= (ba)^nb(ab) \\
&= (ba)^n(ba)b \\
&= (ba)^{n+1}b. \\
\end{align}$$

### Solution

Suppose for group element $a$ and $b$ we have $|ab| = n$. Then $(ab)^n = e$. Moreover, by multiplying on the left by $b$, we see that $b(ab)^n = be = b$. By our lemma, $(ba)^nb = b$. By canceling on the right, $(ba)^n = e$ which implies $|ba| \le n$.

Let $k \le n$ be the least positive integer such that $(ba)^k = e$. Using similar arguments as before, we see $a(ba)^k = a$. By our lemma, $(ab)^k a = a$ and $(ab)^k = e$. So, $|ab| = n \le k$. It must then be that $k = n$ and $|ba| = n$.
