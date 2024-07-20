## Exercise 1

Before approaching the first problem, it helps to establish a couple of trivial lemmas:

**Lemma 1.1** $A \cap A = A$.

*Proof* Suppose $x \in A$, then $x$ is in $A$ and $A$. Thus, $A \subset A \cap A$. Trivially, if $x \in A \cap A$ then $x \in A$ and $A \cap A \subset A$. By double inclusion, $A \cap A = A$.

**Lemma 1.2** $A \cup (A \cap B) = A$.

*Proof* Suppose $x \in A \cup (A \cap B)$, then $x$ is in $A$ or $x$ is in $A$ and $B$. Either case, $x$ is in $A$ so $A \cup (A \cap B) \subset A$. Similarly, if $x$ is in $A$, then clearly $x$ is in $A \cup (A \cap B)$ so $A \cup (A \cap B) = A$.

1: Prove:

  - $A \cap (B \cup C) = (A \cap B) \cup (A \cap C)$.
  - $A \cup (B \cap C) = (A \cup B) \cap (A \cup C)$.

*Proof*. We will prove the first statement through double inclusion. Suppose $x \in A \cap (B \cup C)$. Then $x\in A$ and $x \in B \cup C$. That is, $x \in B$ or $x \in C$. If $x \in B$, then $x \in A \cap B$; otherwise, $x$ is in $C$ and consequently in $A \cap C$. Whatever the case, $x$ is in $A \cap B$ or $A cap C$. Symbolically, $x \in (A \cap B) \cup (A \cap C)$ and $A \cap (B \cup C) \subset (A \cap B) \cup (A \cap C)$. Suppose $x \in (A \cap B) \cup (A \cap C)$, then $x \in A \cap B$ or $x \in A \cap C$. If $x \in A \cap B$, then $x$ is in $A$ and $B$; otherwise, $x$ is in $A$ and $C$. Either way, $x$ is in $A$, and is in $B$ or $C$. That is, $x \in A \cap (B \cup C)$ and $(A \cap B) \cup (A \cap C) \subset A \cap (B \cup C)$. By double inclusion, we have $A \cap (B \cup C) = (A \cap B) \cup (A \cap C)$.

For the second statement, we may show equivalence directly. By our previous work (in the first statement), we know 

$$
\begin{align}
(A \cup B) \cap (A \cup C) &= ((A \cup B) \cap A) \cup ((A \cup B) \cap C) \\
                           &= (A \cap A) \cup (A \cap B) \cup (A \cap C) \cup (B \cap C). \\
\end{align}
$$

Through our lemmas, we also know

$$
\begin{align}
(A \cup B) \cap (A \cup C) &= A \cup (A \cap B) \cup (A \cap C) \cup (B \cap C) \\
                           &= A \cup (A \cap C) \cup (B \cap C) \\
                           &= A \cup (B \cap C). \\
\end{align}
$$
