tags:: linear algebra

-
-
- **Definition**: Suppose $A \in \mathbb{R}^{n \times m}$, if $G \in \mathbb{R}^{m \times n}$ satisfies
  
  $$ AGA = A, $$
  
  then $G$ is called a _pseudo inverse_ of $A$.
- ## Moore-Penrose Inverse
- **Definition**: Suppose $A \in \mathbb{R}^{n \times m}$, if $G \in \mathbb{R}^{m \times n}$ satisfies
  
  $$ AGA = A, GAG = G, (AG)^T = AG, (GA)^T = GA$$
  
  then $G$ is called the _Moore-Penrose inverse_ of $A$.
- **Proposition**: Moore-Penrose inverse is unique.
- **Theorem (use SVD to compute Moore-Penrose inverse)**: Suppose $A$ has the SVD decomposition as $A = U \Sigma V^T$, then its Moore-Penrose inverse is
  
  $$ A^+ = V\Sigma^{-1}U^T $$