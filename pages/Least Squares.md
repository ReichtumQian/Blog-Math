tags:: Linear Algebra, Numerical Linear Algebra

-
- **Least Squares Problem**: Given matrix $A \in \mathbb{R}^{m \times n}$ and $b \in \mathbb{R}^m$, find $x \in \mathbb{R}^n$ such that
  
  $$ \|b - Ax\|_2 = \min \limits_{y \in \mathbb{R}^n} \|Ay - b\|_2 $$
-
- ## Sum Form
- **Theorem**: Find matrix $K$ to minimize
  
  $$ J(\tilde{K}) = \sum\limits_{n = 1}^N \|\Psi(y(n)) - \tilde{K} \Psi(x(n))\|^2_2, $$
  
  where $\Psi: \mathbb{R}^d \rightarrow \mathbb{R}^M$ is a vector function. It can be written into a matrix form $\|\mathbf{Y} - \tilde{K}\mathbf{X}\|_F^2$, where
  
  $$ \mathbf{X} = \left[
  \begin{array}{cccc}
    \Psi(x(1))&\Psi(x(2))&\cdots&\Psi(x(N))
  \end{array}
  \right], \quad \mathbf{Y} = \left[
  \begin{array}{cccc}
    \Psi(y(1))&\Psi(y(2))&\cdots&\Psi(y(N))
  \end{array}
  \right],$$
  
  suppose $XX^T$ is non-sigular, then the solution is
  
  $$ K =  YX^T(XX^T)^{-1}.$$
  
  **Proof.** Denote $J(\tilde{K}) = \|\mathbf{Y} - \tilde{K} \mathbf{X}\|_F^2$, take the derivative of $\tilde{K}$ yields
  
  $$ \frac{\partial J(\tilde{K})}{\partial \tilde{K}} = -2 (\mathbf{Y} - \tilde{K} \mathbf{X})\mathbf{X}^T, $$
  
  let the derivative be zero, and we have $\tilde{K} = \mathbf{Y}\mathbf{X}^T(\mathbf{X} \mathbf{X}^T)^{-1}$.
-
-
- ## References
- [Least squares - Wikipedia](https://en.wikipedia.org/wiki/Least_squares)
-