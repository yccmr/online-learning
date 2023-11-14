# Online Convex Optimization

*Online Convex Optimization* (*OCO*) can be considered as a repetitive game between the player/algorithm and the environment/adversary. Denote the convex decision space by $\mathcal{C}$, the convex loss function by $f: \mathcal{C} \rightarrow \mathbb R$, the time horizon by $T$. For $t = 1, 2, ..., T$: 

- Algorithm: Picks a decision vector $\boldsymbol{w}_t \in \mathcal{C}$,
- Adversary: Picks a convex loss function $f_t$, and send \textit{feedback} to the algorithm,
- Algorithm: Suffer from loss, learn, and adapt from the feedback.

We use *regret* to measure the performance of an algorithm:

$$
\text{Regret}_T \coloneqq .
$$

This note will give a brief introduction on the following basic concepts in OCO:

- What's OCO?

- OCO Algorithms

- Experts Problem

- Lower Bound of OCO

- Beyond General Convexity Assumptions