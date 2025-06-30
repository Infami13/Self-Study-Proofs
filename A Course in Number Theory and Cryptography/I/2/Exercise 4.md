# Lemma

**Lemma.** If $\lfloor n / p \rfloor = q$, then $n = qp + r$ for some integer $r$ such that $0 \le r \lt p$. Effectively, floor division refers to the quotient in Euclidean division.

*Proof.* Suppose $\lfloor n / p \rfloor = q$. Then $q$ is the greatest integer such that $q \le n/p,$ or $qp \le n.$ Simultaneously, by Euclidean division, we may express $n = q \prime p + r$ for some $r$ such that $0 \le r \lt p.$ Overall, we have

$$qp \le n = q \prime p + r \lt q \prime p + p.$$

By subtracting $q \prime p$ from all sides of our inequality, we see that

$$qp - q \prime p \le r \lt p$$
$$(q - q \prime)p \le r \lt p.$$

Immediately, we must have $q - q \prime \le 0$, otherwise we arrive at a contradiction ($r$ cannot be simultaneously greater than or equal to a positive multiple of $p$ and less than $p$). However, if $q - q \prime \lt 0$ then $q \lt q \prime.$ Given $q$ is the greatest integer such that $q \le n/p,$ then $n/p > q \prime$. This then implies

$$
\begin{align}
n &= qp \\

\end{align}
$$

# Part A





### Scrap
We proceed with induction. For our base case where $n = 2$, we have $n! = 2! = 2$. When $p = 2$, we can verify that $\alpha = \lfloor n/p \rfloor + \lfloor n/p^2 \rfloor \cdots  = 1$. Indeed $p^\alpha | 2$ but $p^{\alpha + 1} = 4 \nmid 2$. Therefore $p^\alpha \parallel 2$. For any other prime $q$, we see that $q > n!$ so $q \nmid n!.$ Further $\lfloor n/{q} \rfloor + \lfloor n/{q}^2 \rfloor \cdots  = 0$. That is to say ${q}^0 \parallel n!.$

For our hypothesis step, we examine $(n+1)! = (n+1) \cdot n!.$ 
