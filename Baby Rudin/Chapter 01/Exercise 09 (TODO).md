## Exercise 9

Suppose $z = a + bi$, $w = c + di$. Define $z < w$ if $a < c$, and also if $a = c$ but $b < d.$ Prove that this turns the set of all complex numbers into an ordered set. Does this ordered set have the least-upper-bound property?

### Solution

To show all members of the complex numbers are comparable under this order, suppose to the contrary that none of the statements $z < w$, $z = w$, $z > w$ is true. Given $z \ne w$, we have $a \ne c$. Further, $z \nless w$ implies $a \nless c$. That is to say $a \ge c$. But $a$ cannot equal $c$ so $a > c$. By a similar argument, we can show $z \ngtr w$ implies $a < c$. We then have $a < c$ and $c < a$ for members $a, c \in (\mathbb{R}, <)$, a contradiction. It must then be the case that at least one statement of $z < w$, $z = w$, $z > w$ holds.

We first show exactly one statement of $z < w$, $z = w$, $z > w$ is true. We know $R$ is ordered under $<$, so one and only one of the statements $a < c$, $a =c$, $a >c$ holds. Suppose $a < c$, we then immediately have $z < w$ by our order for complex numbers. By contrapositive, $z \ge w$ implies $a \ge c$. That is to say only $z < w$ holds as either $z = w$ or $z > w$ would mean $a \ge c$, a contradiction. With similar work, we may show $a > c$ implies $z > w$ and only $z > w$ is true. We are then left with the case $a =c$. If $b < d$ then $z < w$. Further, $z \ge w$ would imply the absurdity $a \ne c$ or $b \ge d$, so only $z < w$ holds. With similar style arguments, we may show $b > d$ ensures only $z > w$ is true; $b = d$ implies only $z = w$ holds.
