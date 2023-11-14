# Online Convex Optimization

*Online Convex Optimization* (*OCO*) can be considered as a repetitive game between the player/algorithm and the environment/adversary. Denote the convex decision space by $\mathcal{C}$, the convex loss function by $f: \mathcal{C} \rightarrow \mathbb R$, the time horizon by $T$. For $t = 1, 2, ..., T$: 

- Algorithm: Picks a decision vector $\boldsymbol{w}_t \in \mathcal{C}$,
- Adversary: Picks and sends a convex loss $f_t$ with **full information** to the algorithm,
- Algorithm: Suffer, learn, and adapt from the loss.

We use *regret* to measure the performance of an algorithm:

$$
\text{Regret}_T \coloneqq \sum_{t=1}^{T} f_t(\boldsymbol{w}_t) - \min_{\boldsymbol{u} \in \mathcal{C}} \sum_{t=1}^{T} f_t(\boldsymbol{u}).
$$


This note will briefly introduce the following basic concepts in OCO:

- What's OCO?

- OCO Algorithms

- Experts Problem

- Lower Bound of OCO

- Beyond General Convexity Assumptions
