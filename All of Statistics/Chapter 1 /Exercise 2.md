## Exercise 2

Prove the statements in equation (1.1).

Before addressing the statements in equation (1.1), we use the following lemma.

**Lemma.** $\sigma$-additivity implies additivity. That is, with disjoint $A_1, A_2, ...$,

$$ P\left(\bigcup_{i=1}^{\infty} A_i\right) = \sum_{i=1}^{\infty} P(A_i) \Rightarrow P(A \cup B) = P(A) + P(B) $$

for disjoint $A$ and $B$.

*Proof.* Suppose $A$ and $B$ are disjoint. We may construct the countable union 

$$\bigcup\limits_{i=1}^{\infty} C_i \textrm{ where } C_1 = A, C_2 = B, \textrm{and } C_i = \emptyset \textrm{ for } i \ge 3.$$  

Similarly, we may also construct

$$\bigcup_{i=1}^{\infty} \beta_i \textrm{ where } \beta_1 = B \textrm{ and } \beta_i = \emptyset \textrm{ for } i \ge 2.$$

With disjoint $C_1, C_2, ...$, we see that

$$P(A \cup B) = P(A \cup B \cup \emptyset \cup \emptyset \cup ...) = P\left(\bigcup_{i=1}^{\infty} C_i\right)$$
