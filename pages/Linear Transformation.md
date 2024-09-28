tags:: Linear Algebra

-
- **Definition**: Assume $D$ is a linear space on the field $\mathbb{P}$, linear map $\mathcal{A}: V \rightarrow V$ is called a _linear transformation_ in $V$.
- **The Matrix of Linear Transformation**: $\mathcal{A}$ is a linear transformation in $V$, if $V = \mathrm{span}\{\epsilon_1,\epsilon_2,\cdots,\epsilon_n\}$, and
  
  $$ (\mathcal{A}(\epsilon_1),\mathcal{A}(\epsilon_2),\cdots,\mathcal{A}(\epsilon_n)) = (\epsilon_1,\cdots,\epsilon_n)A, $$
  
  then $A$ is called the _matrix_ of $\mathcal{A}$ under the basis $(\epsilon_1,\cdots,\epsilon_n)$.
- **The Coordinate after Transformation**: Assume the matrix of linear transformation $\mathcal{A}$ under $(\epsilon_1,\cdots,\epsilon_n)$ is $A$, $\alpha \in V$ has the coordinates $X$ under this basis, then $\mathcal{A}\alpha$ has the coordinates $AX$.
  
  **Proof**: Direct computation yields
  
  $$ \mathcal{A}\alpha = \mathcal{A}(x_1\epsilon_1+ \cdots + x_n\epsilon_n) = \mathcal{A}(\epsilon_1,\cdots,\epsilon_n)X = (\epsilon_1,\cdots,\epsilon_n)AX. $$
-