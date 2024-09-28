tags:: numerical solution of PDE

-
- **Problem**: Given $T > 0$, $\mathbf{f} : \mathbb{R}^N \times [0, T] \rightarrow \mathbb{R}^N$, and $\mathbf{u}_0 \in \mathbb{R}^N$, the _initial value problem_ is to find $\mathbf{u}(t) \in \mathcal{C}^1$ such that
  
  $$
  \begin{cases}
  \mathbf{u}(0) = \mathbf{u}_0\\
  \mathbf{u}^{\prime}(t) = \mathbf{f}(\mathbf{u}(t), t), \quad \forall t \in [0,T]
  \end{cases}
  $$
- **Notation**: The initial condition is $\mathbf{U}^0 = \mathbf{u}_0$ and the time-step $k$ is uniform.
- **Forward Euler Method**: The forward Euler's method is given by
  
  $$ \mathbf{U}^{n+1} = \mathbf{U}^n + k\mathbf{f}(\mathbf{U}^n, t_n). $$