-
- Consider the dynamical system
  
  $$ x(n+1) = f(x(n)), \quad x(n) \in \mathcal{M}, \quad n \geq 0, $$
  
  where $(\mathcal{M}, \mathcal{F}, \rho)$ is measure space ($\mathcal{M} \subseteq \mathbb{R}^d$ is the underlying space, $\mathcal{F}$ is the $\sigma$-algebra, $\rho$ is the measure).
- **Observables**: Here we consider the Hilbert space
  
  $$ L^2(\mathcal{M}, \rho) = \left\{ \psi: \mathcal{M} \rightarrow \mathbb{C}: \quad \|\psi\|_{L^2(\mathcal{M}, \rho)} < \infty \right\}, $$
  
  and for the dynamical system, for all $\psi \in L^2(\mathcal{M}, \rho)$, we call it an _observable_.
- ## Definition
- **Koopman Operator**: For any function of state $\psi \in L^2(\mathcal{M}, \rho)$, _Koopman operator_ maps the observable to another observable
  
  $$ \mathcal{K} \psi = \psi \circ f, $$
  
  satisfies $\mathcal{K}: L^2(\mathcal{M}, \rho) \rightarrow L^2(\mathcal{M}, \rho)$.
- **Koopman Operator is Linear**: It's not hard to see, since Koopman operator is a linear transformation.
- **Koopman Operator Defines a New Dynamical System**: Let $\psi(n) \in L^2(\mathcal{M}, \rho)$, then
  
  $$ \psi(n+1) = \mathcal{K} \psi(n). $$
  
  This new dynamical system governs the evolution of observables.
-
- ## Algorithms to Solve Koopman Operator
- [[EDMD]]: Compute a finite dimensional approximation of the Koopman operator.
-
-
- ## References
-
-