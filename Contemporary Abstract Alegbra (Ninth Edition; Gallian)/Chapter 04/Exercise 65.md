# Exercise 65

For prime $p$ and positive integer $n$, consider each integer between $1$ and $p^n$. Clearly, there are $p^n$ such integers. In other words, there are at most $p^n$ integers between $1$ and $p^n$ that are coprime with $p^n$.

Now consider multiples of $p$ that are less than or equal to $p^n = p^{n-1}p$. That is, consider $1p$, $2p$, $3p$, ..., $p^{n-1}p$. Given $p$ divides each of its multiples, it is clear that these $p^{n-1}$ multiples are not coprime with $p^n$.  As such, there are at least $p^{n-1}$ integers between $1$ and $p^n$ that are not coprime with $p^n$.

On the other hand, take integer $a$ where $1 \le a \le p^n$ and suppose $a$ and $p$ are not coprime. That means they share some non-one positive divisor, say $d$. Seeing that $d | p^n$, then for some integer $k$ we have $dk = p^n$. If $d$ were a product of primes other than $p$, then the integer $dk$ would have another prime factorizations other than $p^n$, which contradicts Theorem 0.3. It must be the case that $p$ is a factor of $d$. With $p | d$ and $d | a$, then $p | a$. That is to say that integers between $1$ and $p^n$ are not coprime with $p^n$ if and only if they are multiples of $p$. Altogether, out of the $p^n$ integers, exactly $p^{n-1}$ integer are not coprime with $p^n$, and $\phi(p^n) = p^n - p^{n-1}$.
