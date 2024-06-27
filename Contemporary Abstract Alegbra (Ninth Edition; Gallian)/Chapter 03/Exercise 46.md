## Exercise

Suppose $a$ belongs to a group and $|a|=5$. Prove that $C(a) = C(a^3)$. Find an element $a$ from some group such that $|a| = 6$ and $C(a) \ne C(a^3)$.

### Solution

Suppose $c \in C(a)$, which means $ac = ca$. It immediately follows 
  $$a^3c = aa(ac) = aa(ca) = a(ac)a = a(ca)a = (ac)aa = (ca)aa = ca^3.$$
That is, $c$ commutes with $a^3$ and $C(a) \subseteq C(a^3)$.

Suppose $c \in C(a^3)$, meaning $a^3c = ca^3$. Multiplying on the left by $a^{-2}$, we have $ac = a^{-2}ca^3$. Further, seeing that $a^5 = e$, then $a^3 = a^{-2}$ and $a^6 = a$. We then observe
  $$ac = a^{-2}ca^3 = a^3ca^3 = ca^3a^3 = ca^6 = ca.$$
Specifically, $c$ commutes with $a$ which implies $C(a^3) \subseteq C(a)$. By double inclusion, $C(a) = C(a^3)$.

For the second part, we examine the dihedral group $D_6$. In particular, take the elements $R_{60}$, $R_{180}$, and $H$ (60-degree rotation, 180-degree rotation, and horizontal flip respectively). Notice that $|R_{60}| = 6$. Further, $R_{60}^3 = R_{180}$ commutes with $H$ but $R_{60}$ does not. Symbolically, $H \in C(R_{60}^3)$ and $H \notin C(R_{6}0)$, which is sufficient to show $C(R_{60}) \ne C(R_{60}^3)$.
