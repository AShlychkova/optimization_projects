## Robust optimization
### Shlychkova Aleksandra 699

**Task:**
In some optimization problems there is uncertainty or variation in the objective and constraint functions, due to parameters or factors that are either beyond our control or unknown. We can model this situation by making the objective and constraint functions $ f_0, ..., f_m$ functions of the optimization variable $x \in R^n$ and a parameter vector $u \in R^k$ that is unknown, or varies. In the stochastic optimization approach, the parameter vector u is modeled as a random variable with a known distribution, and we work with the expected values $E_u f_i(x, u)$. In the worst-case analysis approach, we are given a set $U$ that $u$  is know to lie in, and we work with the maximum or worst-case values $sup_{u \in U} f_i(x, u)$. To simplify the discussion, we assume there are no equality constraints.


[1] Stochastic optimization. We consider the problem:
* minimize_ $(E f_0(x, u) )$
* subject to_ $(Ef_i(x, u) < 0, i=1,..,m) $
where the expectation is with respect to u. Show that if $f_i$ are convex in x for each $u$, then this stochastic optimization problem is convex.


[2] Worst-case optimization. We consider the problem:
* minimize  $sup_{u \in U} f_0(x, u) $
* subject to  $sup_{u \in U} f_i(x, u) < 0, i=1,..,m, $
Show that if $f_i$ are convex in x for each u, then this worst-case optimization problem is convex.


[3] Finite set of possible parameter values. The observations made in parts (a) and (b) are most useful when we have analytical or easily evaluated expressions for the expected values $E f_i(x, u) $ or the worst-case values $sup_{u \in U} f_i(x, u)$. Suppose we are given the set of possible values of the parameter is finite, i.e., we have $u \in \{u_1, ..., u_N\}.$ For the stochastic case, we are also given the probabilities of each value: $prob(u=u_i)=p_i$, where $p\in R^N, p > 0, 1^Tp=1$. Intheworst-case formulation, we simply take $U \in \{u_1, ..., u_N\}$.
Show how to set up the worst-case and stochastic optimization problems explicitly.