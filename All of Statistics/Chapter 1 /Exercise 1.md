## Exercise 1
Fill in the details of the proof of Theorem 1.8. Also, prove the monotone decreasing case.

**Theorem 1.8.** If $A_n \rightarrow A$ then
$$P(A_n) \rightarrow P(A)$$
as $n \rightarrow \infty$.

*Proof.* Suppose that $A_n$ is monotone increasing so that $A_1 \subset A_2 \subset \cdots$. Left $A = \lim_{n\to\infty} A_n = \bigcup\nolimits_{i=1}^\infty A_i$. Define $B_1 = A_1$, $B_2 = \lbrace \omega\in\Omega : \omega\in A_2, \omega\notin A_1 \rbrace$, $B_3 = \lbrace\omega\in\Omega : \omega\in A_3, \omega\notin A_2, \omega\notin A_1\rbrace,...$ It can be shown that $B_1, B_2,...$ are disjoint, $A_n=\bigcup\nolimits_{i=1}^n A_i = \bigcup\nolimits_{i=1}^n B_i$ for each $n$ and $\bigcup\nolimits_{i=1}^\infty B_i=\bigcup\nolimits_{i=1}^\infty A_i$. From Axiom 3,

$$P(A_n)=P\left(\bigcup_{i=1}^n B_i\right)=\sum_{i=1}^n P(B_i)$$

and hence, using Axiom 3 again,

$$\lim_{n\to\infty} P(A_n) = \lim_{n\to\infty} \sum_{i=1}^n P(B_i) = \sum_{i=1}^\infty P(B_i) = P \left(\bigcup_{i=1}^\infty B_i \right) = P(A_i).$$
### Solution

To prove $B_1, B_2, ...$ are disjoint, suppose to the contrary there is some $\omega\in B_i\cap B_j$ where $i\ne j$. Without loss of generality, assume $i < j$. By the construction of $B_i$, we have $\omega\in A_i$. Similarly, by the construction of $B_j$, we have $\omega\in A_j$. Further, seeing that $\omega\in B_j$, then $\omega \notin A_k$ for any $k < j$. Particularly, $\omega\notin A_i$ for $i < j$, a contradiction. It must then be that $B_i\cap B_j = \emptyset$ when $i\ne j$. That is, the $B_1, B_2,...$ are disjoint.

To show $A_n = \bigcup\nolimits_{i=1}^n A_i = \bigcup\nolimits_{i=1}^n B_i$, we start by proving $A_n = \bigcup\nolimits_{i=1}^n A_i$ by double inclusion. Suppose $\omega\in A_n$, then $\omega\in \bigcup\nolimits_{i=1}^n A_i$ by definition, so $A_n \subset \bigcup\nolimits_{i=1}^n A_i$. Now suppose $\omega\in \bigcup\nolimits_{i=1}^n A_i$, then $\omega$ is in some $A_i$ for $1 \le i \le n$. However, recall that $A_1 \subset A_2 \subset \cdots \subset A_n$, so if $\omega\in A_i$ for some $i \le n$, then $\omega\in A_n$. Thus, $\bigcup\nolimits_{i=1}^n A_i \subset A_n$. Moreover, $A_n = \bigcup\nolimits_{i=1}^n A_i$. 

To demonstrate $\bigcup\nolimits_{i=1}^n A_i = \bigcup\nolimits_{i=1}^n B_i$, we use double inclusion again. Suppose $\omega\in \bigcup\nolimits_{i=1}^n B_i$, then $\omega$ is in some $B_i$, say $B_k$. Then $\omega\in A_k$ by the constuction of $B_k$. Given $\omega$ is in some $A_i$, we have $\omega\in \bigcup\nolimits_{i=1}^n A_i$, so $\bigcup\nolimits_{i=1}^n B_i \subset \bigcup\nolimits_{i=1}^n A_i$. For the other inclusion, we use induction. In the base case $n=2$, if $\omega\in \bigcup\nolimits_{i=1}^2 A_i$ then $\omega\in A_1$ or $\omega\in A_2$. In the case $\omega\in A_1$, we have $\omega\in B_1$ as $A_1 = B_1$. Otherwise if $\omega\notin A_1$, it must be that $\omega\in A_2$. Here, we have $\omega\in B_2$ as $B_2 = A_2 \backslash A_1$. Either way, $\omega\in \bigcup\nolimits_{i=1}^2 B_i$ and $\bigcup\nolimits_{i=1}^n A_i \subset \bigcup\nolimits_{i=1}^n B_i$ for $n=2$. For the induction step, assume $\bigcup\nolimits_{i=1}^k A_i = \bigcup\nolimits_{i=1}^k B_i$ holds. Suppose $\omega\in \bigcup\nolimits_{i=1}^{k+1} A_i$. Then $\omega\in \bigcup\nolimits_{i=1}^k A_i$ or $\omega\in A_{k+1}$. If the former is true, then $\omega\in \bigcup\nolimits_{i=1}^k B_i \subset \bigcup\nolimits_{i=1}^{k+1} B_i$ by our hypothesis. Otherwise, $\omega\in A_{k+1}$ and no other $A_i$, so $\omega\in B_{k+1} \subset \bigcup\nolimits_{i=1}^{k+1} B_i$. Thus, $\bigcup\nolimits_{i=1}^n A_i \subset \bigcup\nolimits_{i=1}^n B_i$. Overall, $A_n = \bigcup\nolimits_{i=1}^n A_i = \bigcup\nolimits_{i=1}^n B_i$.

To show $\bigcup\nolimits_{i=1}^\infty A_i = \bigcup\nolimits_{i=1}^\infty B_i$, suppose $\omega\in \bigcup\nolimits_{i=1}^\infty A_i$. That is, suppose $\omega$ is in some $A_i$. Let $k$ be the smallest integer such that $\omega\in A_k$ so that $\omega\notin A_j$ for any $j < k$. By construction of $B_k$, we have $\omega\in B_k$. In turn, $\omega\in \bigcup\nolimits_{i=1}^\infty B_i$. Now suppose $\omega\in \bigcup\nolimits_{i=1}^\infty B_i$. Then $\omega\in B_k$ for some $k$. By construction of $B_k$, we have $\omega\in A_k$, so $\omega\in \bigcup\nolimits_{i=1}^\infty A_i$. By double inclusion, $\bigcup\nolimits_{i=1}^\infty A_i = \bigcup\nolimits_{i=1}^\infty B_i$.

Finally, to prove the other case, take $A_n$ as monotone decreasing so that $A_1 \supset A_2 \supset \cdots$. In turn, we have $A_1^c \subset A_2^c \subset \cdots$, analogous to the monotone increasing case. Let $A = \lim_{n\to\infty} A_n = \bigcap\nolimits_{i=1}^\infty A_i$. Note that $\left(\bigcap\nolimits_{i=1}^\infty A_i\right)^c = \bigcup\nolimits_{i=1}^\infty A_i^c$ (see Exercise 3<sup>†</sup>), so $A^c = (\bigcap\nolimits_{i=1}^\infty A_i)^c = \bigcup\nolimits_{i=1}^\infty A_i^c$.  Define $B_1 = A_1^c$, $B_2 = \lbrace\omega\in A_2^c : \omega\notin A_1^c\rbrace$, $B_3 = \lbrace\omega\in A_3^c : \omega\notin A_2^c, \omega\notin A_1^c\rbrace$, and so on. Using similar arguments as before, we have $B_1, B_2, \dots$ are disjoint, $A_n^c = \bigcup\nolimits_{i=1}^n A_i^c = \bigcup\nolimits_{i=1}^n B_i$ for each $n$ and $\bigcup\nolimits_{i=1}^\infty A_i^c = \bigcup\nolimits_{i=1}^\infty B_i$. Using Axiom 3 and the properties of $P$, we have

$$\begin{align}
\lim_{n\to\infty} P(A_n) &= \lim_{n\to\infty}(1-P(A_n^c)) \\
&= 1 - \lim_{n\to\infty} P(A_n^c) \\
&= 1 - \lim_{n\to\infty} P\left(\bigcup_{i=1}^n B_i\right) \\
&= 1 - \lim_{n\to\infty} \sum_{i=1}^n P(B_i) \\
&= 1 - \sum_{i=1}^\infty P(B_i) \\
&= 1 - P\left(\bigcup_{i=1}^\infty B_i\right) \\
&= 1 - P(A^c) \\
&= P(A) \\
\end{align}$$






