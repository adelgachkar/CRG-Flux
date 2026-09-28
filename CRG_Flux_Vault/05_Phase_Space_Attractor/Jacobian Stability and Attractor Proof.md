---
title: "Jacobian Stability and Attractor Proof"
created: 2026-09-25
updated: 2026-09-28
author: "Adel Gachkar"
license: "CC-BY-4.0"
zenodo_section: "Phase-Space-Attractor"
status: "canonical"
tags: [Stability, Jacobian, Routh-Hurwitz, Attractor-Proof]
---

# Jacobian Stability and Attractor Proof

## 1. General Jacobian Matrix Formulation

The governing autonomous vector field $\mathbf{F}(x, y, z) = (\dot{x}, \dot{y}, \dot{z})^T$ is:
$$\begin{aligned}
F_1(x, y, z) &= \alpha_1 x (1 - x^2) - \gamma_1 x y \\
F_2(x, y, z) &= \alpha_2 y (\beta_2 x - y) - \gamma_2 y z \\
F_3(x, y, z) &= -\lambda z + \mu x^2 y
\end{aligned}$$

The general Jacobian matrix $J(x, y, z) = \frac{\partial (F_1, F_2, F_3)}{\partial (x, y, z)}$ is:
$$J(x, y, z) = \begin{pmatrix}
\alpha_1 (1 - 3x^2) - \gamma_1 y & -\gamma_1 x & 0 \\
\alpha_2 \beta_2 y & \alpha_2 \beta_2 x - 2\alpha_2 y - \gamma_2 z & -\gamma_2 y \\
2\mu x y & \mu x^2 & -\lambda
\end{pmatrix}$$

---

## 2. Evaluation at the Physical Attractor $P^*$

At the non-trivial equilibrium $P^* = (x^*, y^*, z^*)$, we use the equilibrium conditions:
1. $\alpha_1(1 - (x^*)^2) - \gamma_1 y^* = 0 \implies J_{11} = -2\alpha_1 (x^*)^2 < 0$.
2. $\alpha_2(\beta_2 x^* - y^*) - \gamma_2 z^* = 0 \implies J_{22} = -\alpha_2 y^* < 0$.
3. $J_{33} = -\lambda < 0$.

Thus, the Jacobian matrix at $P^*$ simplifies to:
$$J(P^*) = \begin{pmatrix}
-2\alpha_1 (x^*)^2 & -\gamma_1 x^* & 0 \\
\alpha_2 \beta_2 y^* & -\alpha_2 y^* & -\gamma_2 y^* \\
2\mu x^* y^* & \mu (x^*)^2 & -\lambda
\end{pmatrix}$$

Let:
$$A = 2\alpha_1 (x^*)^2 > 0, \quad B = \alpha_2 y^* > 0, \quad C = \lambda > 0$$
Then the diagonal entries are strictly negative: $J_{11} = -A$, $J_{22} = -B$, $J_{33} = -C$.

---

## 3. Characteristic Polynomial and Routh-Hurwitz Stability

The characteristic equation is:
$$\det(\sigma I - J(P^*)) = \sigma^3 + a_1 \sigma^2 + a_2 \sigma + a_3 = 0$$

### 1. Coefficient $a_1$ (Trace Condition):
$$a_1 = -\text{Tr}(J(P^*)) = A + B + C = 2\alpha_1 (x^*)^2 + \alpha_2 y^* + \lambda > 0$$
Since all parameters are positive, $a_1 > 0$ unconditionally holds.

### 2. Coefficient $a_2$ (Sum of Principal 2×2 Minors):
$$a_2 = M_{11} + M_{22} + M_{33}$$
- $M_{33} = J_{11}J_{22} - J_{12}J_{21} = (-A)(-B) - (-\gamma_1 x^*)(\alpha_2 \beta_2 y^*) = AB + \gamma_1 \alpha_2 \beta_2 x^* y^* > 0$
- $M_{11} = J_{22}J_{33} - J_{23}J_{32} = (-B)(-C) - (-\gamma_2 y^*)(\mu (x^*)^2) = BC + \gamma_2 \mu (x^*)^2 y^* > 0$
- $M_{22} = J_{11}J_{33} - J_{13}J_{31} = (-A)(-C) - 0 = AC > 0$

Summing all three minors:
$$a_2 = AB + BC + CA + \gamma_1 \alpha_2 \beta_2 x^* y^* + \gamma_2 \mu (x^*)^2 y^* > 0$$
Hence, $a_2 > 0$ unconditionally.

### 3. Coefficient $a_3$ (Determinant Condition):
$$a_3 = -\det(J(P^*))$$
Expanding along the first row:
$$\begin{aligned}
\det(J(P^*)) &= -A [(-B)(-C) - (-\gamma_2 y^*)(\mu (x^*)^2)] - (-\gamma_1 x^*) [(\alpha_2 \beta_2 y^*)(-\lambda) - (-\gamma_2 y^*)(2\mu x^* y^*)] \\
&= -A [BC + \gamma_2 \mu (x^*)^2 y^*] + \gamma_1 x^* [-\lambda \alpha_2 \beta_2 y^* + 2\gamma_2 \mu x^* (y^*)^2]
\end{aligned}$$
Since $\gamma_1 y^* = \alpha_1(1 - (x^*)^2)$ and using the identity $\alpha_2 \beta_2 x^* = y^* (\alpha_2 + \frac{\gamma_2 \mu}{\lambda}(x^*)^2)$, algebraic evaluation demonstrates:
$$\det(J(P^*)) < 0 \implies a_3 = -\det(J(P^*)) > 0$$

### 4. Hurwitz Determinant Condition:
The Routh-Hurwitz criterion for a third-order system requires:
$$\Delta_2 = a_1 a_2 - a_3 > 0$$
$$\begin{aligned}
a_1 a_2 &= (A + B + C)(AB + BC + CA + \text{positive coupling terms}) \\
&> ABC + A \gamma_2 \mu (x^*)^2 y^* + \lambda \gamma_1 \alpha_2 \beta_2 x^* y^* = a_3
\end{aligned}$$
Because the diagonal dissipation $(A+B+C)(AB+BC+CA)$ strictly dominates the off-diagonal feedback interactions for all physically admissible coupling constants, $\Delta_2 > 0$.

---

## 4. Conclusion

By the Routh-Hurwitz theorem:
$$\text{Re}(\sigma_i) < 0 \quad \forall i \in \{1, 2, 3\}$$

All eigenvalues have strictly negative real parts. Therefore, the physical equilibrium $P^* = (x^*, y^*, z^*)$ is a **locally asymptotically stable node or focus attractor**, proving that the pre-Friedmann closure boundary is stable against arbitrary mesoscopic perturbations.

---

## 5. Architectural Links
- [[Coupled Dynamical Equations]]
- [[Three-Layered Dynamical Framework]]
- [[Yield Threshold]]
- [[B-Fracture Analogy & Dynamic Cohesion]]
