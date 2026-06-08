# Exercise 20

Take $g \in G$. We know that $g^{35} = e$. By Theorem Corollary 2 of 4.1, we know if $g^{35} = e$, then $|g|$ divides $35$. For this to be possbile, the order of $g$ must be 1, 5, 7, or 35. That is to say each element of $G$ has order 1, 5, 7, or 35.

We know that exactly one element in $G$ has order of 1, namely the identity, so we consider all other elements. Additionally, if $G$ has any elements of order $35$, then we are done as such an element would generate the group. We are then interested in groups where non-identity elements have order of 5 or 7.

Suppose $G$ has a mix of non-identity elements with order 5 and 7. Then we may select such elements $x$ and $y$ such that $|x|=5$ and $|y|=7$. Again, as $xy \in G$ it must be the case $xy$ has order 1, 5, 7, or 35. We may show $xy \ne e$ as otherwise would imply $y = x^{-1}$, which would mean $y^5 = (x^{-1})^5 = e$, which would contradict the order of $y$. Additionally, given $G$ is commutative, we also see that $(xy)^5 = x^5y^5 = ey^5 = y^5$ and $(xy)^7 = x^7y^7 = x^5x^2e = ex^2e = x^2$. We are left with $|xy|=35$. 

We now consider cases where all 34 non-identiy elements have order $5$. By the Corollary of Theorem 4.4, we know the number of elements of order $5$ is a multiple of $\phi(5) = 4$. Albeit, $34$ is not a multiple of $4$, so no such groups exists. Similarily, we consider cases where all non-identiy elements have order $7$. For this group, the number of elements of order $7$ is a multiple of $\phi(7)=6$; however, $34$ is not a multple of $6$. As such, $G$ must have a mix of non-identity elements with order 5 and 7, and therefore an element of order 35.

The argument does not work if $35$ is replaced with $33 = 3 \cdot 11$ as there may be the case where a group has 1 identity element and all other $16\phi(3) = 16\cdot2 = 32$ elements of order 3.
