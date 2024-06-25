## Exercise
(1969 Putnam Competition) Prove that no group is the union of two proper subgroups. Does the statement remain true if "two" is replaced by "three"?

### Solution
Suppose to the contrary we may form group $G$ with the union of two proper subgroups $H$ and $K$. Symbolically, this means $G = H \cup K$. Suppose $H \subseteq K$. Then, $H \cup K = K < G$. More explicitly, we see $H \cup K \ne G$. So it must be the case that $H \not\subseteq K$ and there is an element $h \in H$ that is not found in $K$. By a similar argument, if we suppose $K \subseteq H$, then $H \cup K \ne G$. As such, there is also an element in $k \in K$ not found in $H$.

Given $k \in K$ and $h \in H$, we have $k^{-1} \in K$ and $h^{-1} \in H$. Furthermore, we also see that $hk \in G = H \cup K$. That is $hk \in H$ or $hk \in K$. However, if $hk \in H$ and $h^{-1} \in H$ then $h^{-1}hk = k \in H$. If $hk \in K$ and $k^{-1} \in K$ then $hkk^{-1} = h \in K$. In either case, we arrive at a contradiction and cannot form a group as the union of two proper subgroups.

To show a group may form from the union of three proper, take $U(8) = \set{ 1, 3, 5, 7 }$ with subgroups $\set{1, 3}$, $\set{1, 5}$, and $\set{1, 7}$.
