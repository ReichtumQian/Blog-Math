tags:: Optimal Control

- ## Optimal Control Formulation
- **The Dynamics**: Consider the ordinary differential equation
  
  $$ \dot{x}(t) = f(t, x(t), \theta(t)), \quad t \in [t_0, t_1], \quad x(t_0) = x_0. $$
  
  Here $x(t) \in \mathbb{R}^d$ is the *state*, $\theta(t) \in \Theta \subset \mathbb{R}^m$ is the *control*, with $\Theta$ the *control set*.
- **The Cost Functional**: We consider functional of the form
  
  $$ J[\theta] = \int_{t_0}^{t_1} L(t, x(t), \theta(t))\mathrm{d} t + \Phi(t_1, x(t_1)), $$
  
  where $L: \mathbb{R} \times \mathbb{R}^d \times \Theta \rightarrow \mathbb{R}$ is called the *running cost*, $\Phi: \mathbb{R} \times \mathbb{R}^d \rightarrow \mathbb{R}$ is called the *terminal cost*.
- **The Bolza Problem of Optimal Control**: The Bolza problem of optimal control is
  
  $$ \inf \limits_{\theta} J[\theta] = \int_{t_0}^{t_1} L(t, x(t), \theta(t))\mathrm{d} t + \Phi (t_1, x(t_1)), $$
  
  such that $\dot{x}(t) = f(t, x(t), \theta(t))$, where $t \in [t_0, t_1]$ and $x(t_0) = x_0$.
- The case where $\Phi = 0$ is called **Lagrange problem**, and the case *L=0* is called a **Mayer problem**.
- **See Also**:
- ## Solution
- [[Pontryagin's Maximum Principle]]
-
-
-
-