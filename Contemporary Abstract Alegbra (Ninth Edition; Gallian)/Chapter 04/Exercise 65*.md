# Exercise 65

For prime $p$ and positive integer $n$, consider each integer between $1$ and $p^n$. Clearly, there are $p^n$ such integers. In other words, there are at most $p^n$ integers between $1$ and $p^n$ that are coprime with $p^n$.

Now consider multiples of $p$ that are less than or equal to $p^n = p^{n-1}p$. That is, consider $1p$, $2p$, $3p$, ..., $p^{n-1}p$. Given $p$ divides each of its multiples, it is clear that these $p^{n-1}$ multiples are not coprime with $p^n$.  As such, there are at least $p^{n-1}$ integers between $1$ and $p^n$ that are not coprime with $p^n$.

On the other hand, take integer $a$ where $1 \le a \le p^n$ and suppose $a$ and $p$ are not coprime. That means there is some positive non-one divisor $d$ such that $\gcd(a, p^n) = d$. Seeing that $d | p^n$, then $dq = p^n$ for some integer $q$. By The Fundamental Theorem of Arithmetic (Theorem 0.3), $d$ and $q$ must be powers of $p$......
