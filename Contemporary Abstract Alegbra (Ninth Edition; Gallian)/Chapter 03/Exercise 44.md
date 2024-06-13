## Exercise
If $H$ is a subgroup of $G$, then by the *centralizer* $C(H)$ of $H$ we mean the set $\Set{x \in G \mid xh = hx \textrm{ for all } h \in H}$. Prove that $C(H)$ is a subgroup of $G$.

### Solution
Given $H$ is a group, it contains identity element $e$, where $eh = he = h$ for each $h \in H$. That is, $C(H)$ contains $e$ and $C(H)$ is non-empty.

Suppose $a, b \in C(H)$. Then $ah = ha$ and $bh = hb$ for any $h \in H$. We then have $(ab)h = a(bh) = a(hb) = (ah)b = (ha)b = h(ab)$. That is, $ab$ commutes with any $h \in H$ and $ab \in C(H)$.

Again, given $a \in C(H)$, then $ah = ha$ for any $h \in H$. Multiplying both sides by $a^{-1}$ on the left and right, we see $a^{-1}aha^{-1} = a^{-1}haa^{-1}$. Or simply, $ha^{-1} = a^{-1}h$ and $a^{-1}$ commutes with any $h \in H$. By the construction of $C(H)$, we have $a^{-1} \in C(H)$. By the Two-Step Subgroup Test, $C(H)$ is a subgroup of $G$.
