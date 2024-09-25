-
-
-
-
- ## Algorithm
- **Problem**: Assume the system is $\mathbf{x}(n+1) = f(\mathbf{x}(n))$, where $\mathbf{x}(n) \in \mathbb{R}^d$, $f: \mathbb{R}^d \rightarrow \mathbb{R}^d$ and $n$ represents the number of step.
- **Data Collection**: Collect a set of data $\{\mathbf{x}_i\}_{i = 1}^N$ and the corresponding next step data $\{\mathbf{y}_i\}_{i = 1}^N$ from the system, satisfying $\mathbf{y}_i = f(\mathbf{x}_i)$.
- **Dictionary Selection**: Pick a proper group of dictionary basis functions $\Psi = \{\psi_1,\cdots,\psi_M\}$, where $\psi_i: \mathbb{R}^d \rightarrow \mathbb{R}$. Take the notation of vector-valued function
  
  $$ \Psi(\mathbf{x}) = \left[
  \begin{array}{cccc}
    \psi_1(\mathbf{x})&\psi_2(\mathbf{x})&\cdots&\psi_M(\mathbf{x})
  \end{array}
  \right]. $$
  
  Note for convience $\Psi(\mathbf{x})$ is a row vector.
- **Dictionary Matrix Construction**: Generate the dictionary matrix
  
  $$
  G = \frac{1}{N} \sum\limits_{i = 1}^N \Psi(\mathbf{x}_i)^T \Psi(\mathbf{x}_i), \quad A = \frac{1}{N} \sum\limits_{i = 1}^N \Psi(\mathbf{x}_i)^T \Psi(\mathbf{y}_i).
  $$
- **Solution**: The finite dimensional approximation of the koopman operator is
  
  $$ K = G^+ A, $$
  
  where $G^+$ is the pseudo-inverse of $G$.
-
- ## References
- [1] A Data–Driven Approximation of the Koopman Operator: Extending Dynamic Mode Decomposition
- [2] Qianxiao Li, Felix Dietrich, Erik M Bollt, Ioannis G Kevrekidis. Extended dynamic mode decomposition with dictionary learning: A data-driven adaptive spectral decomposition of the Koopman operator
-