# Exercise 16

$|a| = |a^2|$ if and only if $|a|$ is odd or infinite. 

Suppose $|a| = |a^2|$. If $|a|$ is infinite, then we are done, so we examine that case where $|a|$ is finite, say $|a|=n.$ By Theorem 4.2, we must have

$$n = |a| = |a^2| = n/\gcd(n,2),$$

which means we must have $\gcd(n,2) = 1$. In other words, $|a| = n$ is odd.

Suppose $|a|$ is infinite. If $|a^2|=n$ were finite, then $(a^2)^n = a^{2n} =e$, which contradicts the infinite order of $a$. As such, $|a^2| = \infty$ and $|a|=|a^2|$.

Lastly, in the finite case, suppose $|a| = n$ is odd. Then by Theorem 4.2 again, we have

$$\lvert a \rvert = n = n/1 = n/\gcd(n,2) = \lvert a^2 \rvert.$$

