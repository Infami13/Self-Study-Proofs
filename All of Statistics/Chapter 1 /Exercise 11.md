# Exercise 11

Suppose $A$ and $B$ are independent events, then $P(AB) = P(A)P(B)$. Recall $P(X) = 1 - P\left(X^C\right)$ for any evident $X$. With this information, we may deduce

$$
\begin{align}
1 - P\left(\left(AB\right)^C\right) &= \left(1 - P\left(A^C\right)\right) \left(1 - P\left(B^C\right)\right) \\
                                    &= 1 - P\left(A^C\right) - P\left(B^C\right) + P\left(A^C\right)P\left(B^C\right). \\                   
\end{align}
$$

With some additional algebraic manipulation, we see that 

$$ 
\begin{align}
-P\left(\left(AB\right)^C\right) &=  - P\left(A^C\right) - P\left(B^C\right) + P\left(A^C\right)P\left(B^C\right) \\
-P\left(A^C\right)P\left(B^C\right) &= - P\left(A^C\right) - P\left(B^C\right) + P\left(\left(AB\right)^C\right) \\
P\left(A^C\right)P\left(B^C\right) &= P\left(A^C\right) + P\left(B^C\right) - P\left(\left(AB\right)^C\right) \\
                                   &= P \left( A^C \cup B^C \right) \\
                                   &= P \left( (AB)^C \right). \\ 
\end{align}
$$
