## Exercise 1

Suppose $x, y \in \mathbb{R}$ and $x < y$. Prove that there exists $i \in \mathbb{R} \setminus \mathbb{Q}$ such that $x < i < y$.

### Lemma

If $x \in \mathbb{Q}$ and $y \in \mathbb{R} \setminus \mathbb{Q}$, then $x + y$ is irrational. Further, if $x \ne 0$ then $xy$ is also irrational.

*Proof*. For our first statement, suppose $x + y$ is rational. Given $\mathbb{Q}$ is a field, then $(-x) + x + y = y$ is also rational, a contradiction.

For our second statement, suppose $x \ne 0$ and $xy$ is rational. Then $x$ is invertible, and we can also attest $x^{-1}xy = y$ is rational, another contradiction.

### Solution

In the case $x$ is rational and $y$ is irrational (or vice versa), we furnish $i = (x + y)/2$ so that $x < i < y.$ Our previous lemma (applied twice) confirms $i$ is irrational.

If $x$ and $y$ are both irrational, the Archimedean property of the reals asserts we may find a rational $q$ such the $x < q < y.$ We then choose $i = (x + q)/2$ so that $x < i < q < y$. As before, our lemma confirms $i$ is irrational.

Lastly, if $x$ and $y$ are rational, we know $0 < y - x$. By the Archimedean property, we have $n(y -x) > \sqrt{2}$ for some natural $n$. That is, $ny > \sqrt{2} + nx$. Choose $i = \sqrt{2}/n + x$ so that $x < i < y$. Recall $1/n$ and $x$ are rational, so $i$ must be irrational by our lemma.

## Exercise 2

Let $E \subset (0, 1)$ be the set of all real numbers with decimal representation using only the digits $1$ and $2$:

$$E \coloneq \Set{x \in (0, 1) : \forall j \in N, \exists d_{-j} \in \Set{1, 2} \textrm{ such that } x = 0.d_{-1}d_{-2}...}$$

Prove that $|E| = |\mathcal{P} (N)|. *Hint*: Consider the function $f:E \rightarrow \mathcal{P} (N)$ such that if $x\in E, x=0.d_{-1}d_{-2}...$,

$$f(x) = \Set{j\in N : d_{-j} = 2}.$$
$\coloneq$
