## Exercise 9

Suppose $z = a + bi$, $w = c + di$. Define $z < w$ if $a < c$, and also if $a = c$ but $b < d.$ Prove that this turns the set of all complex numbers into an ordered set. Does this ordered set have the least-upper-bound property?

### Solution

We first show exactly one statement of $z < w$, $z = w$, $z > w$ is true. We know $R$ is ordered under $<$, so one and only one of the statements $a < c$, $a =c$, $a >c$ holds. Suppose $a < c$, we then immediately have $z < w$ by our order for complex numbers. By contrapositive, $z \ge w$ implies $a \ge c$. That is to say only $z < w$ holds as either $z = w$ or $z > w$ would mean $a \ge c$, a contradiction. With similar work, we may show $a > c$ implies $z > w$ and only $z > w$ is true. We are then left with the case $a =c$. If $b < d$ then $z < w$. Further, $z \ge w$ would imply the absurdity $a \ne c$ or $b \ge d$, so only $z < w$ holds. With similar style arguments, we may show $b > d$ ensures only $z > w$ is true; $b = d$ implies only $z = w$ holds.

Let $v = e + fi$; we proceed by showing the transitive property of $<$ with complex numbers. Suppose $z < w$ and $w < v$. Given $z < w$ and $w < v$, then $a \le c$ and $c \le e$. If $a < c < e$, then we immediately see $z < w < v$. If $a = c < e$, then $a = c$ would imply $b < d$ (any other choice of $b = d$ or $b > d$ would lead to a contradiction). With $a=c, b < d,$ and $c < e$, we can assert $z < w < v$. By similar logic, we can show $a < c = e$ also implies $z < w < v$. Finally, if $a = c = e$ then we must have $b < d < f$, in which case $z< w< v$. Seeing that both trichotomy and transitivity hold, then $<$ turns the set of all complex numbers into an ordered set.

To show this ordered set does not have the least-upper-bound property, it suffices to find a subset of the complex numbers that does not have a supremum with the given order. Take the set

$$X = \Set{ \frac{n}{n+1} \mid n \in \mathbb{N} }.$$

Indeed, $x \le 1$ for each $x \in X$ so $X$ is bounded above. Further, for any bound $z = a + bi$ we must have $a \ge 1$ (otherwise for sufficiently large $n$ we may find $a < n/n+1$)*. Nevertheless, if $z$ is a bound for $X$ then $w = a + (b - 1)i$ is also a bound for $X$, yet clearly $w < z$. That is to say, for any bound of $X$ we may construct another bound that is strictly less and $X$ has no least upper bound.

* - This follows from the Archimedean property of the reals; recall $a$ and $n/n+1$ are real. Tf $a < n/n+1$ under the context of real order, then $z < x$ for some $x \in X$ under the context of our complex order (a contradiction to the idea $z$ is a bound for $X$).
