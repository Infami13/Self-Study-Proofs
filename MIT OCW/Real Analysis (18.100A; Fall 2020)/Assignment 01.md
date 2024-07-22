## Exercise 1

### Supporting Lemmas

**Lemma 1.1** $A \cap A = A$.

*Proof*. Suppose $x \in A$, then $x$ is in $A$ and $A$. Thus, $A \subset A \cap A$. Trivially, if $x \in A \cap A$ then $x \in A$ and $A \cap A \subset A$. By double inclusion, $A \cap A = A$.

**Lemma 1.2** $A \cup (A \cap B) = A$.

*Proof*. Suppose $x \in A \cup (A \cap B)$, then $x$ is in $A$ or $x$ is in $A$ and $B$. Either case, $x$ is in $A$ so $A \cup (A \cap B) \subset A$. Similarly, if $x$ is in $A$, then clearly $x$ is in $A \cup (A \cap B)$ so $A \cup (A \cap B) = A$.

### Problem
Prove:

  - $A \cap (B \cup C) = (A \cap B) \cup (A \cap C)$.
  - $A \cup (B \cap C) = (A \cup B) \cap (A \cup C)$.

Before approaching the first problem, it helps to establish a couple of trivial lemmas:

### Solution

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

## Exercise 2

### Problem

Prove by induction that $n < 2^n$ for all $n \in \mathbb{N}$.

### Solution

*Proof*. Let $P(n)$ describe the statement $n < 2^n$; we will use induction to show $P(n)$ is true for each natural number $n$. In the base case $n = 1$, we have $n = 1 < 2 = 2^1 = 2^n$ and the base case holds. That is, $P(1)$ is true. Next, for the hypothesis step, assume $P(n)$ is true; i.e., $n < 2^n$. It then follows $n + 1 < 2^n + 1 < 2^n + 2^n = 2\cdot 2^n = 2^{n+1}$. In summary, $P(n+1)$ is true whenever $P(n)$ is true. By induction, $n < 2^n$ for all $n \in \mathbb{N}$.

## Exercise 3

### Problem

Show that for a finite set $A$ of cardinality $n$, the cardinality of $\mathcal{P} (A)$ is $2^n$.

### Solution

*Proof*. We proceed with induction. Suppose for the base case that $|A| = 1$. Then there exists a bijective function $f$ that maps $A$ to ${1}$. That is, $A$ has a single element, say $a_1$. Thus, only $\emptyset$ and ${a_1}$ are subsets of $A$ and $\mathcal{P} (A) = \set{\emptyset , {a_1}}$. We may then furnish a trivial bijection $g$ from $\mathcal{P} (A)$ to $\set{1, 2}$ by setting $g(\emptyset) = 1$ and $g({a_1}) = 2$. Thus, $|\mathcal{P} (A)| = 2^1 = 2^n$.

For the hypothesis step, assume $|A| = n$ implies that $\mathcal{P} (A)$ is $2^n$. Now assume that $A$ has cardinality $n + 1$. That is, there is a bijection $f$ from $A$ to $\set{1, 2, ..., n + 1}$. Given $f$ is bijective, then $f^{-1}(n + 1)$ maps to a unique element in $A$, say $a_{n+1}$. Consider the set $B = A \setminus {a_{n+1}}$, a set that has a bijection with $\set{1, 2, ..., n}$ (namely $f \setminus (a_{n + 1}, n + 1)$). Seeing that $|B| = n$, then $|\mathcal{P} (B)| = 2^n$ by our hypothesis. That is, there is a bijection $g$ that maps all the subsets of $B$ to the set $\set{1, 2, ..., 2^n}$. Let us define the function $h$ that maps $\mathcal{P} (A)$ to $\set{1, 2, ..., 2^{n + 1}}$ as follows

$$
h(x) = \begin{cases}
g(x) & \text{if } a_{n + 1} \notin x,\\
2^n + g(x \setminus a_{n + 1}) & \text{otherwise}.
\end{cases}
$$

Note that $A$ and $B$ differ by one member $a_{n + 1}$, so subsets of $A$ either take the form $\beta$ or $\beta \cup \set{a_{n + 1}}$, where $\beta$ is a subset of $B$. All that remains is to show $h$ is bijective.

Suppose $h(x_1) = h(x_2)$. If $h(x_1) = h(x_2) > 2^n$, then $2^n + g(x_1 \setminus a_{n + 1}) = 2^n + g(x_2 \setminus a_{n + 1})$ and $g(x_1 \setminus a_{n + 1}) = g(x_2 \setminus a_{n + 1})$. Given that $g$ is bijective, we know that $x_1 \setminus a_{n + 1} = x_2 \setminus a_{n+1}$. Further, $x_1 = x_2$ seeing that $a_{n+1}$ is in both $x_1$ and $x_2$. If $h(x_1) = h(x_2) <= 2^n

Given $A$ is finite and has cardinality $n$, there exists a bijective function $f$ that maps $A$ to $N = \set{1, 2, ..., n}$.

## Exercise 4

### Problem

Prove that $n^3 + 5n$ is divisible by 6 for all $n \in \mathbb{N}$.

### Solution

*Proof*. We will prove this statement throught induction. For the base case $n = 1$, we have $n^3 + 5n = 1^3 + 5 \cdot 1 = 1 + 5 = 6 = 6 \cdot 1$, which is clearly divisible by $6$. Now assume that $n^3 + 5n$ is divisible by $6$. We then have $(n+1)^3 +5(n + 1) = n^3 + 3n^2 + 3n + 1 + 5n + 5 = n^3 + 5n + 3n^2 + 3n + 6 = n^3 + 5n + 3(n^2 + n + 2)$. By our hypothesis, we know $n^3 + 5n = 6m$ for some integer $m$. 
