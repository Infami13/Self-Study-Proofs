# Exercise 38

We claim $\mu = \textrm{lcm}(m, n)$ is the generator for the group $\langle m \rangle \cap \langle n \rangle$. To prove this, we first show that any integer $a$ is a multiple of $\mu$ if and only if $a$ is a multiple of $m$ and $n$.

Suppose $a$ is a multiple of $\mu$. Then $a = q_1\mu$. However, $\mu$ is a multiple of both $m$ and $n$, so $\mu = q_2m$ and $\mu = q_3n$. In turn, $a = q_1q_2m = q_1q_3n$ and $a$ is a multiple of $m$ and $n$. Now suppose $a$ is a multiple of $m$ and $n$. By Exercise 10 of Chapter 0, we already know this implies $a$ is a multiple of $\mu$. We now tie this result with the original problem.

Suppose $b \in \langle m \rangle \cap \langle n \rangle$. Then $b$ is some multiple of $\mu$ by our hypothesis. As such, $b$ is a multiple of $m$ and $n$, which means it also appears in both $\langle m \rangle$ and $\langle n \rangle$. On the other hand, suppose $b \in \langle m \rangle$ and $b \in \langle n \rangle$. Then $b$ is a multiple of $m$ and $n$, which means $b$ is a multiple of $\mu$. As such, $b \in \langle m \rangle \cap \langle n \rangle$.
