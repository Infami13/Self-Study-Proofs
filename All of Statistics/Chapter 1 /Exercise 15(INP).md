# Exercise 15

__Note:__ This appears to be a variation of the 'Boy or Girl Paradox'.

We may construct our sample space like so

$$ \Omega =  \left\\{ \omega = (\omega_1, \omega_2, \omega_3) : \omega_i \in \set{0, 1} \right\\},$$

where $1$ denotes a child with blue eyes, and $0$ denotes a child with non-blue eyes. Additionally, the order of our sample elements is defined by the age of the children, where $\omega_1$ refers to the youngest child. For example, the tuple $(1, 1, 0)$ refers to a family where the youngest child has blue eyes; the middle child, blue; the oldest, non-blue.

Let $\Phi$ denote the proability of a child having blue eyes<sup>1</sup>. We know $\Phi(1) = \frac{1}{4}$ and $\Phi(0) = \frac{3}{4}$ Given eye color is independent between children

## Part A

We examine two events here: the event $B_1$ where at least one child has blue eyes, and the event $B_2$ where at least two children have blue eyes. There are ${3 \choose 1} = 3$ ways for exactly one child to have blues eyes, ${3 \choose 2} = 3$ for exactly two to have blue eyes, and ${3 \choose 3} = 1$ ways for all children to have blue eyes. 


1 - The probability $\Phi$ operates under the sample space $\set{0, 1}$ while probability $P$ operates under the sample space $\Omega = \set{0, 1}^3$.
