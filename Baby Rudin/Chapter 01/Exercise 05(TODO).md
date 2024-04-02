## Exercise
Let $A$ be a nonempty set of real numbers which is bounded below. Let $-A$ be the set of all numbers $-x$, where $x\in A$. Prove that

$$\inf A = -\sup (-A).$$

### Lemma
Suppose $b$ is a lower bound of $A$. Then $-b$ is an upper bound of $-A$. Moreover, if $A$ is bounded below, then $-A$ is bounded above.

*Proof.* Given $b$ is a lower bound of $A$, for any $a\in A$ we have $b \le a$. Consequently, $-a \le -b$. By construction of $-A$, we have $a' \le -b$ for any $a' = -a \in -A$. That is to say, $-b$ is an upper bound of $-A$.

### Solution
To show $-\sup (-A)$ is a lower bound of $A$, note that for each $x \in A$, we have $-x \in -A$. By our lemma, $-A$ is bounded above, which then means $-A$ has a least upper bound $\sup (-A)$. So, $-x \le \sup (-A)$ and $-\sup (-A) \le x$ for each $x\in A$. More explicitly, $-\sup (-A)$ is a lower bound of $A$ so $- \sup (-A) \le \inf A$.

To then show $-\sup (-A)$ is the greatest lower bound of $A$, suppose to the contrary that $-\sup (-A) \lt \inf A$. Then there exists a real number $b$ such that $-\sup (-A) \lt b \lt \inf A$. Given $b \lt \inf A$, then $b$ is a lower bound of $A$. Albeit, $-\sup (-A) \lt b$ means $-b \lt \sup (-A)$ and $-b$ is not a upper bound of $-A$, a contradiction to our lemma. It must then be $\inf A = -\sup (-A)$.
