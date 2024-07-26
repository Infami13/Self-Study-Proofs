## Exercise 1

### Problem
Let $F$ be an ordered field and $x, y, z \in F$. Prove if $x < 0$ and $y < z$, then $xy > xz$.

### Solution

Given $x < 0$, then $-x > 0$ by Proposition 1.1.8 (*i*). Further, if $y < z$, then $y + (-y) < z + (-y)$ by Definition 1.1.7. Using the axioms of an ordered field, we may algebraically assert $z - y > 0$. Using Definition 1.1.7, we have $-x(z - y) > -x0$ or $-xz + xy > 0$. Finally, by adding $xz$ to both sides, we find $xy > xz$ as desired.

## Exercise 2

### Problem

Let $S$ be an ordered set. Let $A \subset S$ be a nonempty finite subset. Then $A$ is bounded. Furthermore, $\inf A$ exists and is in $A$ and $\sup A$ exists and is in $A$. Hint: Use induction.

### Solution

Suppose, for the base case, that $|A| = 1$. Then $A$ has a single element, say $a$. Clearly, $a \le a$. That is to say, $a$ is greater than or equal to every element of $A$, so $a$ is an upper bound of $A$; similarly, $a$ is less than or equal to every element of $A$, so $a$ is also a lower bound of $A$. To show $a = \sup A$, we know $\sup A$ is the least upper bound of $A$, so $\sup A$ is an upper bound of $A$ and namely $\sup A \ge a$. However, we know $a$ is an upper bound of $A$, so $\sup A \le a$. By trichotomy, we must have $a = \sup A$ and $\sup A \in A$. A similarly styled argument can show $\inf A \in A$.

Now suppose $|A|=n$ implies $A$ is bounded and $\inf A, \sup A \in A$. If $A = S$ there is nothing to prove, so we may assume $A$ is a proper subset of $S$. That is, we may choose $s \in S$ such that $s \notin A$ and examine $B = A \cup {s}$, where $|B| = n + 1$. For each $a \in A$, we must have $s < a$ or $s > a$. If $s < \inf A$, then $s$ is a lower bound for $A$ and $s \le a$ for each $a \in A$. By the way we constructed $B$, we have $s \le b$ for each $b \in B$ (of course $s \le s$), so $s$ is a lower bound for $B$.
