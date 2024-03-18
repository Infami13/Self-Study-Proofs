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
