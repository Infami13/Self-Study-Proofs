# Exercise 1

## Part A

If $p^{\alpha}\parallel a$, then there exists an integer $d$ such that $p^{\alpha}d = a$. Similarly, because $p^{\beta}\parallel b$, there exists an integer $e$ such that $p^{\beta}e = b$. We then have $p^{\alpha + \beta}de = p^{\alpha}dp^{\beta}e = ab$, which means $p^{\alpha + \beta} | ab$.

To show $p^{\alpha + \beta} \parallel ab$, suppose to the contrary that $p^{\alpha + \beta + 1} | ab$. That is, $p^{\alpha + \beta + 1}k = p^{\alpha + \beta}de$. By multiplicative cancellation of the integers, we have the more simple form $pk = de$, meaning $p | de$. Seeing that $p$ is prime, then $p | d$ or $p | e$. If $p | d$, then $pq = d$ for some $q$, which then implies $p^{\alpha + 1}q = a$. However this is an absurdity as $p^{\alpha}$ exactly divides $a$, so $p$ cannot divide $d$. A similar argument can show $p$ cannot divide $e$ either. Therefore, $p^{\alpha + \beta + 1}$ cannot divide $ab$. We are left with $\alpha + \beta$ being the greatest power of $p$ that divides $ab$.

Now suppose $\alpha < \beta$. Then there is some positive $\gamma$ such that $\alpha + \gamma = \beta$. Further, $p^{\beta} = p^{\alpha + \gamma} = p^{\alpha}p^{\gamma}$. Notice that $a \pm b = p^{\alpha}d \pm p^{\beta}e =  p^{\alpha}d \pm p^{\alpha}p^{\gamma}e = p^{\alpha}(d \pm p^{\gamma}e)$. This immediately implies $p^{\alpha} | a \pm b$.

Again, for the sake of contradiction, suppose $p^{\alpha + 1} | a \pm b$. That is to say, $p^{\alpha + 1}\lambda = a \pm b$ for some integer $\lambda$. We then have, $p^{\alpha + 1}\lambda = p^{\alpha}(d \pm p^{\gamma}e)$. By multiplicative cancellation, $p\lambda = d \pm p^{\gamma}e$. Then by additive cancellation, $p\lambda \mp p^{\gamma}e = d$. Of course, $p | p\lambda$ and $p | p^{\gamma}e$, so $p | p\lambda \mp p^{\gamma}e = d$. However, we have already seen that $p | d$ is an impossibility. We are left with $p^{\alpha}$ exactly dividing $a \pm b$.

## Part B
Take $a = 4$ and $b = 12$ so that $2^2 \parallel 4$ and $2^2 \parallel 12$, meaning $p = 2$ and $\alpha = 2$. We then have $a + b = 16$. However, notice that even though $2^2 | 16$ we also have $2^4 | 16$. This means $\alpha = 2$ is not the greatest power of $p$ that divides $a + b$.
