## Exercise

Prove that if $a$ is the only element of order 2 in a group, then $a$ lies in the center of the group.

### Solution

Let $G$ be a group where $a\in G$ is the only element within that has order 2. Further, let $g\in G$. We must then have $gag^{-1} \in G$. We see 

$$(gag^{-1})^2 = (gag^{-1})(gag^{-1}) = gag^{-1}gag^{-1} = gaag^{-1} = gg^{-1} = e.$$

This means the element $gag^{-1}$ has order $2$ or less. However, if $|gag^{-1}| = 1$ then $gag^{-1} = e$, which then implies $a=e$ and contradicts $|a|=2$. We are left with $|gag^{-1}| = 2$, but the only element in the group with order $2$ is $a$, so $gag^{-1} = a$. Consequently, $ga = ag$ for arbitrary $g$. Thus, $a \in Z(G)$.
