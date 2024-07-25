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

### Solution

*Proof*. We will prove the first statement through double inclusion. Suppose $x \in A \cap (B \cup C)$. Then $x\in A$ and $x \in B \cup C$. That is, $x \in B$ or $x \in C$. If $x \in B$, then $x \in A \cap B$; otherwise, $x$ is in $C$ and consequently in $A \cap C$. Whatever the case, $x$ is in $A \cap B$ or $A \cap C$. Symbolically, $x \in (A \cap B) \cup (A \cap C)$ and $A \cap (B \cup C) \subset (A \cap B) \cup (A \cap C)$. Suppose $x \in (A \cap B) \cup (A \cap C)$, then $x \in A \cap B$ or $x \in A \cap C$. If $x \in A \cap B$, then $x$ is in $A$ and $B$; otherwise, $x$ is in $A$ and $C$. Either way, $x$ is in $A$, and is in $B$ or $C$. That is, $x \in A \cap (B \cup C)$ and $(A \cap B) \cup (A \cap C) \subset A \cap (B \cup C)$. By double inclusion, we have $A \cap (B \cup C) = (A \cap B) \cup (A \cap C)$.

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

*Proof*. Suppose for the base case $n = 1$ that $|A| = n = 1$. Then, we know from Exercise 0.3.5 that $A$ has exactly $1$ member, say $a_1$. That is, $A = \set{a_1}$ and has exactly two subsets $\emptyset$ and $\set{a_1}$. In turn, $\mathcal{P} (a) = \set{\emptyset, \set{a_1}}$ and $\mathcal{P} (A)$ has $2$ members. Again, by Exercise 0.3.5, we then know that $|\mathcal{P} (A)| = 2 = 2^1 = 2^n$.

Assume $|A| = n$ implies  $|\mathcal{P} (A)| = 2^n$. Now suppose $|A| = n + 1$. Consider the set $B$ that has all but one member of $A$, say $a_{n+1}$. That is, $B = A \setminus \set{a_{n+1}}$ and $B$ has $n$ members. Given $|B| = n$, then $|\mathcal{P} (B)| = 2^n$ by our hypothesis. Further, given membership is binary (an object is either in or not in a set), we may partition subsets of $A$ into two categories: those that contain $a_{n + 1}$ and those that do not. Notice that if $\alpha \subset A$ and $a_{n+1} \notin \alpha$, then $\alpha \subset A \setminus \set{a_{n+1}} = B$. That is, the set of subsets of $A$ that do not contain $a_{n+1}$ is exactly $\mathcal{P} (B)$. Let $\frak{P}$ be the set of subsets of $A$ that do contain $a_{n + 1}$. Trivially, we define the bijection $f: \mathcal{P} (B) \rightarrow \frak{P}$ through $f(x) = x \cup \set{a_{n + 1}}$, which means $|\mathcal{P} (B)| = |\frak{P}|$. That is, $A$ has $2^n$ subsets that do not contain $a_{n+1}$ and $2^n$ that do contain $a_{n + 1}$ (and no other subsets). So $A$ has $2 \cdot 2^n = 2^{n + 1}$ subsets and $|\mathcal{P} (A)| = 2^{n + 1}$ as desired.

## Exercise 4

### Supporting Lemma

**Lemma 4.1**. $n^2 + n + 2$ is even for every $n \in \mathbb{N}$.

*Proof*. If $n$ is even, then $n = 2m$ for some integer $m$. It follows $n^2 + n + 2 = (2m)^2 + 2m + 2 = 4m^2 + 2m + 2 = 2(2m^2 + 2m + 2)$; hence, $n^2 + n + 2$ is even. If $n$ is odd, then $n = 2m + 1$ for some integer $m$ and $n^2 + n + 2 = (2m + 1)^2 + 2m + 1 + 2 = 4m^2 + 4m + 1 + 2m + 3 = 4m^2 + 6m + 4 = 2(2m^2 + 3m +2)$ and $n^2 + n + 2$ is even.

### Problem

Prove that $n^3 + 5n$ is divisible by 6 for all $n \in \mathbb{N}$.

### Solution

*Proof*. We will prove this statement through induction. For the base case $n = 1$, we have $n^3 + 5n = 1^3 + 5 \cdot 1 = 1 + 5 = 6 = 6 \cdot 1$, which is clearly divisible by $6$. Now assume that $n^3 + 5n$ is divisible by $6$. We then have

$$(n+1)^3 +5(n + 1) = n^3 + 3n^2 + 3n + 1 + 5n + 5 = n^3 + 5n + 3n^2 + 3n + 6 = n^3 + 5n + 3(n^2 + n + 2).$$

By our hypothesis, we know $n^3 + 5n = 6m$ for some integer $m$. By our lemma, we know $n^2 + n + 2 = 2k$ for some integer $k$. We then have $(n+1)^3 +5(n + 1) = 6m + 3(2k) = 6m + 6k = 6(m + k)$ and $6$ divides $(n+1)^3 +5(n + 1)$.

## Exercise 5

### Problem

Give an example of a countably infinite collection of finite set $A_1, A_2, ...$, whose union is not a finite set.

### Solution

Let $S$ be a collection of sets $A_1, A_2, ...$ such that $A_k = \set{k}$ for each natural number $k$. More explicitly, $S = \set{\set{1}, \set{2}, ...}$. Of couse, each set in $S$ is finite with a cardinality of $1$. To show that $S$ is countably infinte, take the function $f: \mathbb{N} \rightarrow S$ defined by $f(x) = \set{x}$. We know $f$ is injective because if $f(x_1) = f(x_2)$, then $\set{x_1} = \set{x_2}$ and $x_1 \in \set{x_2}$. Seeing that $\set{x_2}$ is singleton, we have $x_1 = x_2$. We also know $f$ is surjective because for any $\set{x} \in S$, we have $x$ as a natural number (by the way $S$ is constructed) in which $f(x)= \set{x}$. Ultimately, $S$ has the same cardinality as $\mathbb{N}$ and is consequently countably infinite.

To then show $U = \bigcup S$ is not finite, it suffices to show that $U = \mathbb{N}$. Suppose $x \in U$, then $x$ is in some member of $S$. Particularly $x \in \set{n}$, where $n$ is a natural number; in which case, $x = n$ and $x \in \mathbb{N}$. Now suppose $x \in \mathbb{N}$. Then $\set{x}$ appears in $S$. Given $\set{x} \in S$, then $x \in U = \bigcup S$. By double inclusion, $U = \mathbb{N}$.

## Exercise 6

### Problem

In this exercise, you will prove that

$$|{q ∈ \mathbb{Q} : q > 0}| = |\mathbb{N}|$$

In what follows, we will use the following theorem without proof:

**Theorem.** Let $q \in \mathbb{Q}$ with $q > 0$. Then

if $q\in \mathbb{N}$ and $q \ne 1$, then there exists unique prime numbers $p_1 < p_2 < \cdots < p_N$ and unique exponents $r_1, ...., r_N \in \mathbb{N}$ such that

$$q = p_1^{r_1}p_2^{r_2}\cdots p_N^{r_N},\tag*{(†)}$$

if $q \notin \mathbb{N}$, then there exist unique prime numbers $p_1 < p_2 < \cdots < p_N$, $q_1 < q_2 < \cdots < q_M$ with $p_i \ne q_j$ for all $i \in \set{1, ..., N}, j \in \set{1, ..., M}$, and unique exponents $r_1, ..., r_N, s_1, ..., s_M \in \mathbb{N}$ such that

$$q = \frac{p_1^{r_1}p_2^{r_2}\cdots p_N^{r_N}}{q_1^{s_1}q_2^{s_2}\cdots q_M^{s_M}}.\tag*{(‡)}$$

Define $f: \set{q \in \mathbb{Q} : q > 0} \rightarrow \mathbb{N}$ as follows: $f(1) = 1$, if $q \in \mathbb{N} \setminus \set{1}$ is given by $(†)$, then

$$f(q) = p^{2r_1}\cdots p_N^{2r_N},$$

and if $q \in \mathbb{Q} \setminus \mathbb{N}$ is given by $(‡)$, then

$$f(q) = p_1^{2r_1}\cdots p_N^{2r_N}q_1^{2s_1-1}\cdots q_M^{2s_M - 1}.$$

- Compute $f(4/15)$. Find $q$ such that $f(q) = 108$.
- Use the **Theorem** to prove that $f$ is a bijection.

### Solution

We start by computing $f(4/15)$. Given 

$$\frac{4}{15} = \frac{2^2}{3^15^1}$$

and $4/15 \notin \mathbb{N}$, we have $f(4/15) = 2^{2 \cdot 2}3^{2\cdot 1 - 1}5^{2\cdot 1 - 1} = 2^43^15^1 = 240.$

On the other hand, we have $108 = 2^23^3 = 2^{2\cdot 1}3^{2 \cdot 2 -1}$. By the way we define $f$, we have $2/9 = 2^1/3^2$ map to $2^{2\cdot 1}3^{2 \cdot 2 -1}$. That is, $f(2/9) = 108$.

*Proof*. To prove $f$ is bijective, we start by showing $f$ is surjective. Suppose $n \in \mathbb{N}$, then $n = 1$ or $n$ is a product of primes by our Theorem. If $n = 1,$ then $f(1) = 1$ by our definition of $f$. Otherwise, by our Theorem again, $n$ may be expressed uniquely as a product of primes $\pi_1^{\rho_1} \cdots \pi_K^{\rho_K}$ for $\pi_1 < \pi_2 < ... < \pi_K$. Given multiplication is commutative for the natural numbers, we may arrange the prime power factors of $n$ such that the first $N$ prime power factors have even exponents (where $\rho_i = 2r_i$ for some $r_i$) and the last $K - N = M$ prime power factors have odd exponents (where $\rho_i = 2s_i -1$ for some $s_i$). That is, $n = p_1^{2r_1} \cdots p_N^{2r_N} q_1^{2s_1 - 1} \cdots q_M^{2s_M - 1}$. We then choose 

$$q = \frac{p_1^{r_1} \cdots p_N^{r_N}}{q_1^{s_1} \cdots q_M^{s_M}}$$

so that $f(q) = p_1^{2r_1} \cdots p_N^{2r_N} q_1^{2s_1 - 1} \cdots q_M^{2s_M - 1} = n$ as desired.

To prove that $f$ is injective, suppose $x \ne y$. Given $x$ and $y$ are positive rationals, we may write them as a quotient of natural numbers; explicitly, $x = a/b$ and $y = \alpha / \beta$. By our Theorem, we may also write $x$ as a quotient of prime powers where prime bases are coprime with one another. We may also express $y$ in a similar fashion. Symbolically,

$$\begin{align}
x &= \frac{a}{b} = \frac{p_1^{r_1} \cdots p_N^{r_N}}{q_1^{s_1} \cdots q_M^{s_M}}, \\
y &= \frac{\alpha}{\beta} = \frac{t_1^{v_1} \cdots t_K^{v_K}}{u^{w_1} \cdots u^{w_J}}
\end{align}$$

In which case,

$$\begin{align}
f(x) &= p_1^{2r_1}\cdots p_N^{2r_N}q_1^{2s_1-1}\cdots q_M^{2s_M - 1}, \\
f(y) &= t_1^{2v_1}\cdots t_K^{2v_K}u_1^{2w_1-1}\cdots u_M^{2w_J - 1}.
\end{align}$$

For brevity, we assume the empty product is $1$ so that we may generalise the following result for whenever $x$ or $y$ is natural. Again $x \ne y$, so $a \ne \alpha$ or $b \ne \beta$. We examine the case that $a \ne \alpha$. By our Theorem, we know $a$ and $\alpha$ may be expressed uniquely (and distinctly) as a product of primes. That is, $a = p_1^{r_1}\cdots p_N^{r_N}$ and $\alpha = t_1^{v_1}\cdots t_K^{v_K}$; and without loss of generality, there is some prime power $p_i^{r_i}$ that divides $a$ but not $\alpha$. It then follows that $p_i^{2r_1} | f(x) = a^2q_1^{2s_1-1}\cdots q_M^{2s_M - 1}$ and either $p_i^{2r_i}$ divides or does not divide $f(y)$. If $p_i^{2r_i}$ does not divide $f(y)$, then we are done as $f(x)$ cannot equal $f(y)$. If $p_i^{2r_i}$ does divide $f(y)$, it must divide some prime power of the form $u_j^{2w_j-1}$; in which case $2r_i < 2w_j - 1$. However, this then implies $u_j^{2w_j-1}$ cannot divide $p_i^{2r_i}$ or any other prime power of $f(x)$—recall $f(x)$ is expressed in such a way that all the prime bases are coprime with one another. We then have, $f(x) \ne f(y)$. A similar approach may show that $b \ne \beta$ also implies $f(x) \ne f(y)$. Overall, $x \ne y$ means $f(x) \ne f(y)$ and $f$ is injective. Given $f$ is a surjection and injection, then $f$ is a bijection.
