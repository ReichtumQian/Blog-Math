-
- **Motivation**: We want to look at what the solution is to a set of initial conditions at a fixed terminal time.
- **Flow Map**: Given a dynamical system $\dot{x}(s) = f(s, x(s))$, and $t \in \mathbb{R}^+$, the flow map $\varphi_t : \mathbb{R}^d \rightarrow \mathbb{R}^d$ is
  
  $$ \varphi_t(x) := x(t), \quad x(0) = x, $$
  
  where initial condition $x$ is the variable.
- **Interpret continuous-time system to discrete-time system**: Given a continuous-time system $\dot{x}(s) = f(s, x(s))$ and its flow map $\varphi_t(x)$, then it can be written into discrete-time form:
  
  $$ \tilde{x}(n+1) = \varphi_t(\tilde{x}(n)), $$
  
  where $\tilde{x}(n) := x(nt)$.
  
  **Proof**. The objective equation is equivalent to $x(nt + t) = \varphi_t(x(nt))$, it is obviously true according to the definition of flow map.
-
-