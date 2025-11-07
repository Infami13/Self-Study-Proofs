## Exercise 2

Prove the statements in equation (1.1).

### Solution

Before addressing the statements in equation (1.1), we use the following lemma.

**Lemma.** Let $\Omega$ be our universal set and let $P$ be a set function with domain $\mathcal{P} (\Omega)$, the powerset of $\Omega$. If $P$ is $\sigma$-additive, then it is additive. That is, if $A$ and $B$ are disjoint and subsets of $\Omega$, then $P(A \cup B) = P(A) + P(B)$.

*Proof.* Suppose $P$ is $\sigma$-additive over $\Omega$. Further, suppose $A$ and $B$ are disjoint and are subsets of $\Omega$. We may construct the countable union $\bigcup\nolimits_{i=1}^{\infty} \beta_i$ where $\beta_1 = B$ and $\beta_i = \emptyset$ for $i \gt 1$. Given the $\beta_i$ are mutually disjoint and $P$ is $\sigma$-additive, we have

$$P(B) = P(B \cup \emptyset \cup \emptyset \cup \cdots) = P\left(\bigcup_{i=1}^{\infty} \beta_i \right) = \sum_{i=1}^{\infty} P(\beta_i)$$

Similarly, we may also construct $\bigcup\nolimits_{i=1}^{\infty} C_i$ where $C_1 = A$, $C_2 = B$, and $C_i = \emptyset$ for $i > 2$. As the $C_i$ are mutually disjoint, we then have

$$
\begin{align}
P(A \cup B) &= P(A \cup B \cup \emptyset \cup \emptyset \cup \cdots) \\
            &= P\left( \bigcup_{i=1}^{\infty} C_i \right) \\
            &= \sum_{i=1}^{\infty} P(C_i) \\
            &= P(A) + P(B) + P(\emptyset) + P(\emptyset) + \cdots \\
            &= P(A) + \sum_{i=1}^{\infty} P(\beta_i) \\
            &= P(A) + P(B). \\
\end{align}
$$

**Theorem.** $P(\emptyset) = 0$.

*Proof.* Notice, by our lemma,

$$P(\emptyset) + P(\emptyset)= P(\emptyset \cup \emptyset) = P(\emptyset) =0 + P(\emptyset)$$

That is, $P(\emptyset) + P(\emptyset) = 0 + P(\emptyset)$. By subtracting $P(\emptyset)$ from both sides, we have $P(\emptyset) = 0$ as desired.

**Theorem.** $A \subset B \Rightarrow P(A) \le P(B)$.

*Proof.* Suppose $A \subset B$. Then there is a set $C = B \backslash A$ where $A \cup C = B$. Further, $A$ and $C$ are disjoint so $P(A) + P(C) = P(A \cup C) = P(B)$. In the case $P(C) = 0$, we have $P(A) = P(B)$. In the other case $P(C) > 0$, we have $P(A) < P(A) + P(C) = P(B)$. In summation, $P(A) \le P(B)$.

**Theorem.** $0 \le P(A) \le 1$.

*Proof.* Note that $0 \le P(A)$ follows directly from the axioms of probability. Also, recall that $P(\Omega) = 1$. Given $A \subset \Omega$, we have $P(A) \le P(\Omega) = 1$. That is, $0 \le P(A) \le 1$.

**Theorem.** $P(A^c) = 1 - P(A)$

*Proof.* Seeing that $A$ and $A^c$ are disjoint, we have $P(A) + P(A^c) = P(A \cup A^c) = P(\Omega) = 1$. That is, $P(A^c) = 1 - P(A)$.

**Theorem.** $A \cap B = \emptyset \Rightarrow P(A \cup B) = P(A) + P(B)$.

*Proof.* Suppose $A \cap B = \emptyset$. By definition, these sets are disjoint, so $P(A \cup B) = P(A) + P(B)$ by our lemma.
