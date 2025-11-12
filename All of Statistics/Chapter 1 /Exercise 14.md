# Exercise 14

We first handle the case where $P(A) = 0$ and utilize common properties of probability (see pg. 6). We know that $AB \subseteq A$ implies $P(AB) \le P(A) = 0$. However, it is also true that $0 \le P(AB)$, so we must have $P(AB) = 0$. All together, we see that $P(AB) = 0 = 0 \cdot P(B) = P(A)P(B)$.

In the case $P(A) = 1$, we first examine that $A \subseteq A \cup B \subseteq \Omega$. This means $P(A) \le P(A \cup B) \le P(\Omega)$, or $1 \le P(A \cup B) \le 1$. It must then be the case that $P(A \cup B) = 1$. From Lemma 1.6, we know $P(A \cup B) = P(A) + P(B) - P(AB)$. Through substitution, we observe $1 = 1 + P(B) - P(AB)$, which asserts $P(AB) = P(B)$. We then have $P(AB) = P(B) = 1 \cdot P(B) = P(A)P(B)$ as desired.

Lastly, we study the case where $A$ is independent of itself. This means $P(AA) = P(A)P(A)$. That is to say, $P(A) = P(A)P(A)$. Of course, this equality holds when $P(A) = 0$ or $P(A) = 1$. To show no other values may satisfy 
this equality, we examine $P(A) \in (0, 1)$. Given $0 < P(A) < 1$, then $0 < P(A)P(A) < P(A) = P(AA)$ which immediately shows $A$ is not independent of itself seeing that $P(AA) \ne P(A)P(A)$.
