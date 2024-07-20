1. Prove:

  - $A \cap (B \cup C) = (A \cap B) \cup (A \cap C)$.
  - $A \cup (B \cap C) = (A \cup B) \cap (A \cup C)$.

We will prove both statements through double inclusion. Starting with the first, suppose $x \in A \cap (B \cup C)$. Then $x\in A$ and $x \in B \cup C$. That is, $x \in B$ or $x \in C$. If $x \in B$, then $x \in A \cap B$; otherwise, $x$ is in $C$ and consequently in $A \cap C$. Whatever the case, $x$ is in $A \cap B$ or $A cap C$. Symbolically, $x \in (A \cap B) \cup (A \cap C)$ and $A \cap (B \cup C) \subset (A \cap B) \cup (A \cap C)$. Suppose $x \in (A \cap B) \cup (A \cap C)$, then $x \in A \cap B$ or $x \in A \cap C$. If $x \in A \cap B$, then $x$ is in $A$ and $B$; otherwise, $x$ is in $A$ and $C$. Either way, $x$ is in $A$, and is in $B$ or $C$. That is, $x \in A \cap (B \cup C)$ and $(A \cap B) \cup (A \cap C) \subset A \cap (B \cup C)$. By double inclusion, we have $A \cap (B \cup C) = (A \cap B) \cup (A \cap C)$.

For the second statement, suppose $x \in A \cup (B \cap C)$. Then $x \in A$ or $x \in B \cap C$. If $x \in A$, then $x$ is in both $A\cup B$ and $A\cup C$. If $x \in B \cap C$, then $x$ is in both $B$ and $C$, which again implies $x$ is in both $A\cup B$ and $A\cup C$. Ultimately, $x \in (A \cup B) \cap (A \cup C)$ and $A \cup (B \cap C) \subset (A \cup B) \cap (A \cup C)$. For the other direction, suppose $x \in (A \cup B) \cap (A \cup C)$. By our previous work (in the first statement), we have 

$\begin{align}
(A \cup B) \cap (A \cup C) &= ((A \cup B) \cap A) \cup ((A \cup B) \cap C) \\
                           &= (A \cap A) \cup (A \cap B) \cup (A \cap C) \cup (B \cap C) \\
                           &= A \cup (A \cap B) \cup (A \cap C) \cup (B \cap C). \\
\end{align}$
