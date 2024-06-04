## Exercise
Suppose $n$ is an even positive integer and $H$ is a subgroup of $Z_n$. Prove that either every member of $H$ is even or exactly half of the members of $H$ are even.

### Solution
If $H$ contains no odd member, we are done. Otherwise, if $H$ contains at least one odd integer (say $a$), let $A$ be the set of all odd integers in $H$ and $B$ be the set of all even integers in $H$. Given every integer is exclusively even or odd, then $A$ and $B$ form a partition of $H$; all that remains is to show $|A| = |B|$. To do this, we will show a bijection exists between $A$ and $B$.

Consider the function $f: A \rightarrow B$ defined by $f(x) = a + x$ for each $x \in A$, where arithmetic is done mod $n$. Note that $f$ is well-defined as the sum of two odd integers is a unique even integer when arithmetic is done under an even modulus. 

Further, $f$ is injective as $f(x) = f(y)$ implies $a + x = a + y$. Seeing that $a \in H$, then $-a \in H$. Adding both sides by $-a$, we see that $a + x = a + y$ then implies $x = y$.

Additionally, $f$ is surjective as for any $b \in B$, choose $x = (-a) + b$ so that $a + x = b$. That is, there is some $x \in A$ such that $f(x) = b$ for any $b \in B$.

Given a bijection exists between $A$ and $B$, we have $|A| = |B|$. Further, seeing that $A$ and $B$ form a partition of $H$, then $|H| = |A| + |B|$. That is, $|H| = |A|+|A| = 2|A|$ and $|A| = |H| / 2$ as desired.
