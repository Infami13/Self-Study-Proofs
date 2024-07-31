## Exercise 1

### Problem
Let $F$ be an ordered field and $x, y, z \in F$. Prove if $x < 0$ and $y < z$, then $xy > xz$.

### Solution

Given $x < 0$, then $-x > 0$ by Proposition 1.1.8 (*i*). Further, if $y < z$, then $y + (-y) < z + (-y)$ by Definition 1.1.7. Using the axioms of an ordered field, we may algebraically assert $z - y > 0$. Using Definition 1.1.7, we have $-x(z - y) > -x0$ or $-xz + xy > 0$. Finally, by adding $xz$ to both sides, we find $xy > xz$ as desired.

## Exercise 2

### Problem

Let $S$ be an ordered set. Let $A \subset S$ be a nonempty finite subset. Then $A$ is bounded. Furthermore, $\inf A$ exists and is in $A$ and $\sup A$ exists and is in $A$. Hint: Use induction.

### Solution

Suppose, for the base case, that $|A| = 1$. Then $A$ has a single element, say $a$. Clearly, $a \le a$. That is to say, $a$ is greater than or equal to every element of $A$, so $a$ is an upper bound of $A$; similarly, $a$ is less than or equal to every element of $A,$ so $a$ is also a lower bound of $A$. To show $a = \sup A$, we know $\sup A$ is the least upper bound of $A$, so $\sup A$ is an upper bound of $A$ and namely $\sup A \ge a$. However, we know $a$ is an upper bound of $A$, so $\sup A \le a$. By trichotomy, we must have $a = \sup A$ and $\sup A \in A$. A similarly styled argument can show $\inf A \in A$.

Now suppose $|A|=n$ implies $A$ is bounded and $\inf A, \sup A \in A$. If $A = S$ there is nothing to prove, so we may assume $A$ is a proper subset of $S$. That is, we may choose $s \in S$ such that $s \notin A$ and examine $B = A \cup \set{s}$, where $|B| = n + 1$. For each $a \in A$, we must have $s < a$ or $s > a$. If $s < \inf A$, then $s$ is a lower bound for $A$ and $s \le a$ for each $a \in A$. By the way we constructed $B$, we have $s \le b$ for each $b \in B$ (of course $s \le s$), so $s$ is a lower bound for $B$ and $s \le \inf B$. However, $s \in B$ implies $s \ge \inf B$, so $s = \inf B$ and $\inf B \in B$. Additionally, $s = \inf B \le \sup A$ so $\sup A$ is a bound for $B$ and $\sup B \le \sup A$ (recall that all non-$s$ elements of $B$ were adopted from $A$). On the other hand, $\sup A \in B$ so $\sup B \ge \sup A$, which means $\sup B = \sup A$ and $\sup B \in B$. If $s > \sup A$, we can follow similar logic in our previous work to show $s = \sup B$, and $\sup B, \inf B \in B$. In the remaining case $\inf A < s < \sup A$, then $\inf A \le b$ for each $b \in B$ yet $\inf A \in B$, so $\inf B = \inf A$. Similarly, we can show $\sup B = \sup A$ and $\sup B \in B$. No matter the case, we have $|B| = n + 1$ implies $\inf B, \sup B \in B$ and hence $B$ is bounded.

## Exercise 3

### Problem

Let $S$ be an ordered set. Let $A \subset S$ and suppose $b$ is an upper bound for $A$. Suppose $b \in A$. Show that $b = \sup A$.

### Solution

Suppose to the contrary that $b \ne \sup A$, meaning $b$ is not the least upper bound of $A$. Then there exists an upper bound $\beta$ of $A$ such that $\beta < b$. However $b \in A$, which means $\beta$ cannot be an upper bound of $A$ (a contradiction). That is to say $b \le \beta$ for every upper bound $\beta$ of $A$. By definition, $b$ is the least upper bound of $A$, notated as $b = \sup A$.

## Exercise 4

### Problem

Let $S$ be an ordered set. Let $A \subset S$ be nonempty and bounded above. Suppose $\sup A$ exists and $\sup A \notin A$. Show that $A$ contains a countably infinite subset.

### Solution

By Exercise 2 above, we know if $A$ is finite, then $\sup A \in A$. By contrapositive, $\sup A \notin A$ implies $A$ must be non-finite. Now suppose $x_1 \in A$, then $x_1 \le \sup A$. We know $x_1 \ne \sup A$ because $\sup A \notin A$, so $x_1 < \sup A$. We may then find an element $x_2 \in A$ such that $x_1 < x_2 < \sup A$. We may then find another element $x_3$ such that $x_2 < x_3 < \sup A$. We may continue this process indefinitely.* We then define $B \subset A$ as $B = \set{x_1, x_2, ...}$ where $x_1 < x_2 < ...$ and define bijection $f: B \rightarrow \mathbb{N}$ in the obvious way, $f(x_n) = n$.** That is, there is a subset $B$ of $A$ that shares cardinality with the natural numbers, hence $B$ is countably infinite. Thus, $A$ contains a countably infinite subset.

\* - Suppose to the contrary we encounter an element $x_n$ where there exists no other element in $A$ that is strictly between $x_n$ and $\sup A$. No element of $A$ may be greater than or equal to $\sup A$, so it must be that $x_n \ge a$ for each $a \in A,$ and $x_n$ is an upper bound for $A$. This then implies $x_n \ge \sup A$, an absurdity.

** - For injectivity, if $f(x_i) = f(x_j)$ then $i = j$ and $x_i = x_j$. For subjectivity, if $k \in \mathbb{N}$ then $f(x_k) = k$.

## Exercise 5

### Problem

Prove the arithmetic-geometric mean inequality. For two positive real numbers $x, y,$

$$ \sqrt{xy} \le \frac{x+y}{2}.$$

Furthermore, equality occurs if and only if $x = y$.

### Solution

Suppose to the contrary that $\sqrt{xy} > (x+y)/2$. Given $x >0$ and $y > 0$, we know that $(x + y)/2 > 0$. We can then assert that $0 < (x + y)/2 < \sqrt{xy}$. Using Proposition 1.1.8 and some algebraic manipulation, we know that

$$\begin{align}
\left( \frac{x+y}{2} \right)^2 &< xy \\
(x + y)^2 &< 4xy \\
x^2 + 2xy + y^2 &< 4xy \\
x^2 - 2xy + y^2 &< 0 \\
(x - y)^2 &< 0.
\end{align}$$

If $x = y$, then $(x - y)^2 = 0$ and $0 < 0$, a contradiction. If $x \ne y$, then $x - y \ne 0$ and we have a contradiction to Proposition 1.1.8.

For the later statement, suppose $\sqrt{xy} = (x + y)/2$. Not unlike our work before (swapping the inequality for an equality), we may show that $(x - y)^2 = 0$, which then implies $x - y =0$, or $x = y$. Now suppose $x = y$, then $\sqrt{xy} = \sqrt{xx} = x$ and $(x + y)/2 = (x + x)/2 = x$. That is $\sqrt{xy} = (x +y)/2$ as desired.

## Exercise 6

### Problem

Let $A$ and $B$ be two nonempty bounded sets of real numbers. Let $C := \set{a+b : a\in A, b\in B}$. Show that $C$ is a bounded set and that

$$ \sup C = \sup A + \sup B \textrm{    and    } \inf C = \inf A + \inf B.$$

### Solution

We know $a \le \sup A$ and $b \le \sup B$ for any $a \in A$ and any $b \in B$. Combining these inequalities together through addition, we see that $a + b \le \sup A + \sup B$ for any $a \in A$ and any $b \in B$. That is to say $\sup A + \sup B$ is an upper bound of $C$, so $\sup C \le \sup A + \sup B$.

On the other hand, for any bound $c$ of $C$ and any arbitrary elements $a \in A$ and $b \in B$, we have $a + b \le c$. Thus, $a \le c - b$ for each $a \in A$ and $c - b$ is an upper bound of $A$. This then means $\sup A \le c - b$. We can then show $b \le c - \sup A$ for each $b \in B$, meaning $c - \sup A$ is an upper bound for $B$. Again, we can then deduce $\sup B \le c - \sup A$, or $\sup A + \sup B \le c$. Given $c$ may be any bound, we assert $\sup A + \sup B \le \sup C$. By these two inequalities, we have $\sup C = \sup A + \sup B$.

A similar style argument may be used to show that $\inf C = \inf A + \inf B$.

## Exercise 7

### Problem

Let

$$E = \set{x \in \mathbb{R} : x > 0 and x^3 < 2}.$$

Prove that $E$ is bounded above. Let $r = \sup E$. Prove that $r >0$ an $r^3=2$. 

### Solution

Suppose $x > 0$. If $x \ge 2$, then $x^3 \ge 8$. By contrapositive, if $x^3 < 2 < 8$ then $x < 2$. That is to say, members of $E$ are bounded above. Further, we have $1 \in E$ as $1 > 0$ and $1^3 = 1 < 2$, so $E$ is nonempty. Given $E$ is bounded above, we know that $r = \sup E$ exists.

Now take a positive real $s$ such that $s^3 < 2$, then $s \in E$. Given $s^3 < 2$, then $s^3 - 2 < 0$. Further, we may choose a positive real $h$ such that $h < \frac{2-s^3}{3s^2+3s+1}$. We know such a real exists given $\frac{2-s^3}{3s^2+3s+1}$ is positive. We may also assume $h < 1$. Estimate,

$$\begin{align}
(s + h)^3 - s^3 &= 3s^2h + 3sh^2+h^3 \\
                &= h(3s^2+3sh+h^2) \\
                &< h(3s^2+3s+1) \tag*{$h<1$}\\
                &< 2 - s^3 \tag*{h < }\\
\end{align}$$



