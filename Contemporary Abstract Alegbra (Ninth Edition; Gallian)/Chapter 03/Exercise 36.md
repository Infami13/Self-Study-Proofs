## Exercise 36

Let $G$ be a group, and let $a\in G$. Prove that $C(a) = C(a^{-1})$.

### Solution

Suppose $g\in C(a)$. Then $a$ commutes with $g$ by the construction of $C(a)$. That is, $ag = ga$. Multiplying both sides by $a^{-1}$ on the left, we see $g = a^{-1}ga$. And by multiplying on the right by $a^{-1}$, we have $ga^{-1} = a^{-1}g$. This means $g$ commutes with $a^{-1}$ and $g\in C(a^{-1})$. So, $C(a) \subseteq C(a^{-1})$.

Suppose $g\in C(a^{-1})$. Then $a^{-1}g = ga^{-1}$. Encapsulating both sides by $a$, we have $aa^{-1}ga = aga^{-1}a$. Simply, $ga = ag$ and $g$ commutes with $a$. As such, $g\in C(a)$ and $C(a^{-1}) \subseteq C(a)$. Thus, $C(a) = C(a^{-1})$.
