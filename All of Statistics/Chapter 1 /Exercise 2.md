## Exercise 2

Prove the statements in equation (1.1).

Before addressing the statements in equation (1.1), we use the following lemma.

**Lemma.** $\sigma$-additivity implies additivity. That is, with disjoint $A_1, A_2, ...$,

$$ P\left(\bigcup_{i=1}^{\infty} A_i\right) = \sum_{i=1}^{\infty} P(A_i) \Rightarrow P(A \cup B) = P(A) + P(B) $$

for disjoint $A$ and $B$.

*Proof.* Suppose $A$ and $B$ are disjoint. We may construct the countable union $\bigcup\nolimits_{i=1}^{\infty} \beta_i$ where $\beta_1 = B$ and $\beta_i = \emptyset$ for $i \gt 1$. We then have

$$P(B) = P(B \cup \emptyset \cup \emptyset \cup \cdots) = P\left(\bigcup_{i=1}^{\infty} \beta_i \right) = \sum_{i=1}^{\infty} P(\beta_i)$$

Similarly, we may also construct $\bigcup\nolimits_{i=1}^{\infty} C_i$ where $C_1 = A$, $C_2 = B$, and $C_i = \emptyset$ for $i > 2$. We then have

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
