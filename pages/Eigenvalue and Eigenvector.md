tags:: Linear algebra

-
- **Definition**: Given matrix $A \in \mathbb{R}^{n \times n}$, if there exist a vector $v \in \mathbb{R}^n$ and a value $\lambda \in \mathbb{R}$ such that
  
  $$ A v = \lambda v, $$
  
  then $v$ is called the _(right) eigenvector_ with _eigenvalue_ $\lambda$.
- ## Properties
- **Proposition**: $A$ and $A^T$ have same eigenvalues.

**Proof**. the eigen polynomial of $A$ and $A^T$ are $\mathrm{det}(A - \lambda I)$, $\mathrm{det}(A^T - \lambda I)$, respectively. By the property of $\mathrm{det}(B) = \mathrm{det}(B^T)$, we have the two eigen polynomials are the same.

- 
- 
- ## Left Eigenvectors
- **Definition**: Given matrix $A \in \mathbb{R}^{n \times n}$, if there exist a vector $w \in \mathbb{R}^n$ and a value $\lambda \in \mathbb{R}$ such that
  
  $$ w^T A  = \lambda w^T, $$
  
  then $w$ is called the _left eigenvector_ with _eigenvalue_ $\lambda$.

- **Theorem**: The left eigenvectors share the same set of eigenvalue with right eigenvector.

  **Proof**. Suppose $w^TA = \lambda w^T$, then $A^T w = \lambda w$. Since $A,A^T$ have same eigen values, which completes the proof.

-
