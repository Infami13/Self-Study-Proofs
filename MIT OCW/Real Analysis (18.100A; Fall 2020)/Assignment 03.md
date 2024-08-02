## Exercise 1

Suppose $x, y \in \mathcal{R}$ and $x < y$. Prove that there exists $i \in \mathcal{R} \setminus \mathcal{Q}$ such that $x < i < y$.

### Lemma

If $x \in mathcal{Q}$ and $y \in \mathcal{R} \setminus mathcal{Q}$, then $x + y$ is irrational. Further, if $x \ne 0$ then $xy$ is also irrational.

*Proof*. For our first statement, suppose $x + y$ is rational. Given $\mathcal{Q}$ is a field, then $(-x) + x + y = y$ is also rational, a contradiction.

For our second statement suppose $x \ne 0$ and $xy$ is rational. Then $x$ is invertible, and we can also attest $x^{-1}xy = y$ is rational, a contradiction.

### Solution

In the case $x$ is rational and $y$ is irrational (or vice versa), we furnish $i = (x + y)/2$ so that $x < i < y.$ Our previous lemma (applied twice) confirms $i$ is irrational.

If $x$ and $y$ are both irrational, the Archimedean property of the reals asserts we may find a rational $q$ such the $x < q < y.$ We then choose $i = (x + q)/2$ so that $x < i < q < y$. As before, our lemma confirms $i$ is irrational.

Lastly, if $x$ and $y$ are rational, we know $0 < y - x$. By the Archimedean property, we have $n(y -x) > \sqrt{2}$ for some natural $n$. That is, $ny > \sqrt{2} + nx$. Choose $i = \sqrt{2}/n + x$ so that $x < i < y$. Recall $1/n$ and $x$ are rational, so $i$ must be irrational by our lemma.

