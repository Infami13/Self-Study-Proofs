# Part A

We proceed with induction. For our base case where $n = 2$, we have $n! = 2! = 2$. When $p = 2$, we can verify that $\alpha = \lfloor n/p \rfloor + \lfloor n/p^2 \rfloor \cdots  = 1$. Indeed $p^\alpha | 2$ but $p^{\alpha + 1} = 4 \nmid 2$. Therefore $p^\alpha \parallel 2$. For any other prime $q$, we see that $q > n!$ so $q \nmid n!.$ Further $\lfloor n/{q} \rfloor + \lfloor n/{q}^2 \rfloor \cdots  = 0$. That is to say ${q}^0 \parallel n!.$

For our hypothesis step, we examine $(n+1)! = (n+1) \cdot n!.$ 
