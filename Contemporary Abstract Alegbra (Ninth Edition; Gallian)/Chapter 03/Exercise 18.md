## Exercise
Suppose that $a$ is a group element and $a^6=e$. What are the possibilities for $|a|$?

### Solution
Let $|a|=n$, then $n \in \lbrace 1, 2, 3, 6 \rbrace$. That is, the potential values of $n$ are exactly the divisors of $6$. To show this, for any divisor $n$ of $6$, we may furnish an integer $q$ such that $nq = 6$. Then $a^6 = a^{nq} = (a^n)^q = e^q = e.$

More formally, we define $n$ as the least positive integer such that $a^n = e$. If $n$ does not divide $6$, then we may write $6 = nq + r$ for some $0 < r < n$. In which case,

$$e = a^6 = a^{nq + r} = a^{nq}a^r = a^r.$$

However, this contradicts the minimality of $|a|=n$. That is, if $n$ does not divide $6$, then $a^6 \ne e$. By contrapositive, if $a^6 = e$, then $n$ divides $6$.
