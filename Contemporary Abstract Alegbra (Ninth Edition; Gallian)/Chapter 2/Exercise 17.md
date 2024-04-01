## Exercise
Let $G$ be a group and let $H = \lbrace x^{-1} | x \in G \rbrace$. Show that $G = H$ as sets.

### Solution
Suppose $a\in G$. Given $G$ is a group, then $a^{-1}\in G$ and $(a^{-1})^{-1}\in H$. Seeing that $(a^{-1})^{-1}$ denotes the inverse of $a^{-1}$, we have $a^{-1}(a^{-1})^{-1} = e$ where $e$ is the identity of $G$. Algebraically (Exercise 26), we see that $(a^{-1})^{-1} = a$. As such, $(a^{-1})^{-1}=a\in H$ so $G \subseteq H$.

Suppose $a\in H$. Then $a = b^{-1}$ for some $b\in G$. Seeing that $G$ is a group, we have $b^{-1}=a\in G$. So, $H \subseteq G$.
