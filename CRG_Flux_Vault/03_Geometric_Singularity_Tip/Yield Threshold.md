---
title: "Yield Threshold and Dynamic Buffer Screening"
created: 2026-09-25
updated: 2026-09-28
author: "Adel Gachkar"
license: "CC-BY-4.0"
zenodo_section: "Geometric-Singularity-Tip"
status: "canonical"
tags: [Yield-Threshold, Plasticity, Buffer-Screening, Discriminant]
---

# Yield Threshold and Dynamic Buffer Screening

> **Sign convention (E4, 2026-09-28):** the canonical reading of the discriminant is
> **Θ_yield > 0 reversible-elastic · Θ_yield ≈ 0 active buffer · Θ_yield < 0 screened/
> closed** — i.e. positive discriminant = remaining elastic capacity. Companion notes
> that write $\Theta_{\text{yield}} = \sigma_y/\kappa_c - \Gamma_{\text{eff}}$ as a
> switch statement follow this same convention; earlier drafts showing
> "Θ_yield < 0" for Regime I were a transcription error now fixed.

## 1. Unified Dynamic Yield Discriminant ($\Theta_{\text{yield}}$)

The transition of the pre-Friedmann boundary from a purely reversible flexoelectric membrane to a dissipative, screening buffer layer is governed by the scalar **Dynamic Yield Discriminant**:

$$\Theta_{\text{yield}}(\sigma, \kappa, \dot{\Phi}) \equiv \left( \frac{\sigma_{\text{vM}}}{\sigma_y} + \frac{\kappa_{\text{eff}}}{\kappa_c} - 1 \right) - \frac{\Gamma_{\text{eff}}(\dot{\Phi})}{\Gamma_0}$$

where:
- $\sigma_{\text{vM}} \equiv \sqrt{\frac{3}{2} s_{ij} s_{ij}}$ is the effective in-plane von Mises stress on the 2D carbon sheet.
- $\sigma_y \approx 100\text{--}130 \text{ GPa}$ is the intrinsic tensile yield limit of defect-free monolayer graphene.
- $\kappa_{\text{eff}} \equiv \sqrt{\frac{1}{2} \kappa_{jk} \kappa_{jk}}$ is the invariant curvature intensity derived from out-of-plane corrugated displacements $w(\mathbf{r})$, with consistent continuum convention $\kappa_{jk} \equiv \partial_j \partial_k w$ (such that cross-thickness strain gradient satisfies $\partial_z \varepsilon_{jk} = -\kappa_{jk}$).
- $\kappa_c \approx 1.5\text{--}2.2 \text{ nm}^{-1}$ represents the threshold curvature inducing spontaneous $sp^2 \to sp^3$ tetrahedral rehybridization.
- $\Gamma_{\text{eff}}(\dot{\Phi}) \equiv \Gamma_0 \left[ 1 + \left( \frac{\dot{\Phi}}{\dot{\Phi}_c} \right)^2 \right]$ is the rate-dependent dynamic dissipative capacity modulated by the pre-Friedmann background scalar field velocity $\dot{\Phi}$.

---

## 2. Regime Transitions Across the Singular Boundary

Linear Elastic → Dynamic Plastic → Topological Pinning

[Pure Flexoelectric] [Buffer Dislocation] [Frozen Attractor]

──────────────────────────────┼──────────────────────────────┼─────────────────────────────►

Θ_yield > 0 │ Θ_yield ≈ 0 │ Θ_yield < 0

(σ < σ_y, κ < κ_c) │ (Buffer Layer Active) │ (J_leak → 0)

| Regime | Mathematical Condition | Continuum Mechanical State | Boundary Charge & Screening |
| :--- | :--- | :--- | :--- |
| **I. Elastic Storage** | $\Theta_{\text{yield}} > 0$ | Pure reversible bending; linear strain gradients; no bond breaking. | Linear dipole polarization $\mathbf{P} = -\mu_{\text{eff}} \nabla^2 w$; zero interface free charge. |
| **II. Self-Regulated Yield** | $\Theta_{\text{yield}} \approx 0$ | Localized plastic flow; dislocation nucleation at puckered crests; energy shedding. | Jump discontinuity $\llbracket \mathbf{\Psi} \rrbracket$ compensated by buffer charge sheet $\sigma_{\text{interface}} = -\llbracket \mathbf{\Psi} \rrbracket \cdot \hat{\mathbf{n}}$. |
| **III. Topological Closure** | $\Theta_{\text{yield}} < 0 \quad (\kappa \to \kappa_{\text{sat}})$ | Re-solidified covalent topology; kinetic dissipation exhausted; frozen curvature core. | Complete screening; external leakage flux extinguished ($J_{\text{leak}} \to 0$); compactification locked. |

---

## 3. Microscopic Origin: $sp^2 \to sp^3$ Bond Reconstruction

At curvature levels approaching $\kappa_c$, the overlap integral between carbon $2p_z$ orbitals drops exponentially while $\sigma\text{-}\pi$ orthogonality breaks down:

$$\Delta E_{\text{barrier}}(\kappa) = \Delta E_0 \left[ 1 - \left( \frac{\kappa}{\kappa_c} \right)^2 \right]^{\alpha}$$

When the localized mechanical driving force overcomes $\Delta E_{\text{barrier}}$, spontaneous tetrahedral bond-flipping occurs, neutralizing the divergent metric stress and serving as the microscopic dissipative sink that prevents divergent singular cusps.

![Curved lattice with bond reconstruction](../Assets/fig_curved_lattice_charge.png)
*Figure 1 — Schematic of $sp^2 \to sp^3$ bond reconstruction under curvature beyond $\kappa_c$ (the microscopic dissipative sink of Regime III). Shared illustration with the flexoelectricity folder; AI-rendered schematic, no computed data.*

---

## 4. Architectural Links
- [[MOC - CRG-Flux Architecture]]
- [[Tip Effect and Local Curvature Tensor]]
- [[Sharpness vs Amplitude Scaling]]
- [[Quantum Flexoelectricity in Bent Graphene]]
- [[B-Fracture Analogy & Dynamic Cohesion]]
- [[Buffer Layer and Non-Equilibrium Transport]]
- [[Effective Stiffness Reconstruction]]
- [[Coupled Dynamical Equations]]
- [[Jacobian Stability and Attractor Proof]]
