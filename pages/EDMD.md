- Preliminaries: [[Koopman Operator]]
-
- Extended dynamic mode decomposition (EDMD) algorithm is a method to estimate a finite-dimensional representation of the Koopman operator $\mathcal{K}$.
-
-
- ## Algorithm
- **Problem Description**: Assume the system is $\mathbf{x}(n+1) = f(\mathbf{x}(n))$, where $\mathbf{x}(n) \in \mathbb{R}^d$, $f: \mathbb{R}^d \rightarrow \mathbb{R}^d$. Pick a group of dictionary basis functions $\Psi = \{\psi_1,\cdots,\psi_M\}$, where $\psi_i: \mathbb{R}^d \rightarrow \mathbb{R}$. Our goal is to find a matrix $K$ that tries to satisfy for all $\mathbf{x}(n), \mathbf{x}(n+1)$ such that

$$ K \left[
  \begin{array}{c}
    \psi_1(\mathbf{x}(n))\\
    \psi_2(\mathbf{x}(n))\\
    \vdots\\
    \psi_M(\mathbf{x}(n))
  \end{array}
\right] = \left[
  \begin{array}{c}
    \psi_1(\mathbf{x}(n+1))\\
    \psi_2(\mathbf{x}(n+1))\\
    \vdots\\
    \psi_M(\mathbf{x}(n+1))
  \end{array}
\right]$$

- **Data Collection**: Collect a set of data $\{\mathbf{x}_i\}_{i = 1}^N$ and the corresponding next step data $\{\mathbf{y}_i\}_{i = 1}^N$ from the system, satisfying $\mathbf{y}_i = f(\mathbf{x}_i)$.
- **Construct Matrix**: Construct two matrixes:

$$ \Psi_X = \left[
  \begin{array}{cccc}
    \Psi(\mathbf{x}_1)&\Psi(\mathbf{x}_2)& \cdots &\Psi(\mathbf{x}_N)
  \end{array}
\right], \quad
\Psi_Y = \left[
  \begin{array}{cccc}
    \Psi(\mathbf{y}_1)&\Psi(\mathbf{y}_2)& \cdots &\Psi(\mathbf{y}_N)
  \end{array}
\right],
$$

where $\Psi(\mathbf{x}_i) = [\psi_1(\mathbf{x}_i), \cdots, \psi_M(\mathbf{x}_i)]^T$.

- **Solution**: We are going to solve a minimization problem

$$ \min \|K \Psi_X - \Psi_Y\|_F $$

which is equivalent to $K = \Psi_Y\Psi_X^+$, where $\Psi_X^+$ is the pseudo-inverse of $\Psi_X$.

- ## Validation
- **Validation**: Pick any $\mathbf{x}(n), \mathbf{x}(n+1)$, and check if

$$ K \left[
  \begin{array}{c}
    \psi_1(\mathbf{x}(n))\\
    \psi_2(\mathbf{x}(n))\\
    \vdots\\
    \psi_M(\mathbf{x}(n))
  \end{array}
\right] = \left[
  \begin{array}{c}
    \psi_1(\mathbf{x}(n+1))\\
    \psi_2(\mathbf{x}(n+1))\\
    \vdots\\
    \psi_M(\mathbf{x}(n+1))
  \end{array}
\right]$$

-
- ## References
- [1] A Data–Driven Approximation of the Koopman Operator: Extending Dynamic Mode Decomposition
- [2] Qianxiao Li, Felix Dietrich, Erik M Bollt, Ioannis G Kevrekidis. Extended dynamic mode decomposition with dictionary learning: A data-driven adaptive spectral decomposition of the Koopman operator
-
