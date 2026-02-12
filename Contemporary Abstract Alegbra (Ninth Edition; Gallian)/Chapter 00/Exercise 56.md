# Exercise 56
With license number $149105267$, we proceed by first computing

$$
\begin{align}
9a_1+8a_2+7a_3+6a_4+5a_5+4a_6+3a_7+2a_8+a_9 &= 9\cdot1+8\cdot4+7\cdot9+6\cdot1+5\cdot0+4\cdot5+3\cdot2+2\cdot6+7 \\
                                            &= 155. \\
\end{align}
$$

We also see that $155 \textrm{ mod } 10 = 5$, affirming the license number is indeed erroneous.

We first explore a specific case as an example. Suppose that the error is in position $2$. We may substitute $4$ in position $2$ with any other single digit number, say $4 + n$ such that $0 \le 4 + n \le 9$. This then means that

$$
\begin{align}
9a_1+8(a_2+n)+7a_3+6a_4+5a_5+4a_6+3a_7+2a_8 +a_9   &= 9\cdot1+8(4+n)+7\cdot9+6\cdot1+5\cdot0+4\cdot5+3\cdot2+2\cdot6 + 7 \\
                                                   &= 9\cdot1+8\cdot4 + 8n +7\cdot9+6\cdot1+5\cdot0+4\cdot5+3\cdot2+2\cdot6 + 7 \\
                                                   &= 9\cdot1+8\cdot4 +7\cdot9+6\cdot1+5\cdot0+4\cdot5+3\cdot2+2\cdot6 + 7 + 8n \\
                                                   &= 155 + 8n. \\
\end{align}
$$

Given the error is in position $2$ (by our hypothesis), we many then find $n$ such that $155 + 8n = 0$ under modulo $10$. In other words, there exists an $n$ such that $155 + 8n = 10q$ for some integer $q$. This then implies $155 = 10q - 8n = 2(5q - 4n)$ and that $155$ is an even number, an absurdity. Our original hypothesis that the error is in position 2 is wrong, and we are left with positions 2, 4, and 6 as options.

We now explore the general case to handle remaining positions. Suppose that the error is in an even position. Notice the coefficients of positions 2, 4, 6, and 8 are even (8, 4, 6, and 2 respectively). That is, the coefficients of even positions take the form $2m$, where $m$ is an integer. Changing the digit in one of these positions introduces an offset of $2mn$ to our original sum of $155$, analogous to our specific example. That is, we are left with finding an $n$ such that $155 + 2mn = 10q$. Again, this is impossible as $155 = 2mn - 10q = 2(mn-5q)$ implies $155$ is even. Therefore, the error cannot be in an even position. 
