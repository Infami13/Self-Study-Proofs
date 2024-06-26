This is a common discussion topic in ring algebra with the integers mod $n$, though the term 'division' is rarely used. It's more common to use 'multiplicative inverses'. That is, if $a$ is an element of some ring $R$, its multiplicative inverse (if it exists) is an element $b$ such that $a \cdot b = 1$, where $1$ is the unity of $R$. The multiplicative inverse of element $a$ is commonly notated as $a^{-1}$.

In the case of integers mod 10, the multiplicative inverse of 3 would be 7 as 3 * 7 = 21 = 1 under mod 10. An analog to division would look something like 

$$5/3 = 5 \cdot 3^{-1} = 5 \cdot 7 = 35 = 5,$$

when arithmetic is done mod 10 (though I doubt the division symbol makes many appearances in literature about rings).

For very large moduli, the extended Euclidean algorithm with Bezout's Identity is often used to find multiplicative inverses (see RSA key generation).
