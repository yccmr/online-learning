# Online Convex Optimization

### Problem Description
*Online Convex Optimization* (*OCO*) can be considered as a repetitive game between the player/algorithm and the environment/adversary. Denote the convex decision space by $\mathcal{C}$, the convex loss function by $f: \mathcal{C} \rightarrow \mathbb R$, and the time horizon by $T$. For $t = 1, 2, ..., T$: 

- Algorithm: Picks a decision vector $\boldsymbol{w}_t \in \mathcal{C}$,
- Adversary: Picks and sends a convex loss $f_t$ with **full information** to the algorithm,
- Algorithm: Suffer, learn, and adapt from the loss.

### Performance Metric & Goal
We use *regret* to measure the performance of an algorithm (compared with the best **fixed** decision in hindsight):

$$
\text{Regret}_T \coloneqq \sum_{t=1}^{T} f_t(\boldsymbol{w}_t) - \min_{\boldsymbol{u} \in \mathcal{C}} \sum_{t=1}^{T} f_t(\boldsymbol{u}),
$$

and the goal is to achieve *sub-linear regret*, i.e., 

$$
\text{Regret}_T \in o(T).
$$

### Note
This note will briefly introduce the following basic concepts in OCO:

- What's OCO?

- OCO Algorithms

- Experts Problem

- Lower Bound of OCO
