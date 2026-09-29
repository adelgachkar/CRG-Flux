---
title: "Quantum Flexoelectricity in Bent Graphene and Curvature Coupling"
created: 2026-09-25
updated: 2026-09-29
author: "Adel Gachkar"
license: "CC-BY-4.0"
zenodo_section: "Experimental-Flexoelectricity"
status: "canonical"
tags: [Flexoelectricity, Graphene, FvK, Strain-Gradient, Curvature-Threshold]
---

# Quantum Flexoelectricity in Bent Graphene and Curvature Coupling

## 1. Executive Summary & Physical Continuum

In low-dimensional Dirac semimetals—predominantly pristine and corrugated monolayer graphene—inversion symmetry breaking occurs dynamically through localized out-of-plane deflections. While uniform strain merely renormalizes the Fermi velocity and acts as a static synthetic gauge field $\mathbf{A}_{\text{pseudo}}$, **strain gradients** $(\nabla \boldsymbol{\varepsilon})$ explicitly break structural centrosymmetry. This generates an intrinsic, non-local flexoelectric polarization field:

$$
\mathbf{P}_{\text{flexo}} = \boldsymbol{\mu} : \nabla \boldsymbol{\varepsilon} = \boldsymbol{\mu} : \nabla \boldsymbol{\kappa}
$$

where $\boldsymbol{\kappa} \equiv -\nabla \nabla w$ represents the local curvature tensor associated with the out-of-plane deflection $w(\mathbf{x})$.

Within the **Pre-Friedmann Closure Framework**, flexoelectric wrinkling is not treated as an isolated nanoscale perturbation. Rather, it serves as the mesoscopic laboratory archetype for geometry-induced charge localization, stress screening, and reactive vacuum polarization. The continuous interplay between bending rigidity $D_0$, nonlinear in-plane stretching $C$, and flexoelectric dipole accumulation drives the system from a linear acoustic response toward a critical buckling/wrinkling regime governed by the curvature scale $\kappa_c$.

![Curved lattice with curvature-localized bound charge](../Assets/fig_curved_lattice_charge.png)
*Figure 1 — Schematic of flexoelectric bound-charge concentration at lattice curvature maxima ($\rho_{\text{bound}} = -\mu_{\text{eff}}\nabla^2\operatorname{Tr}\kappa$). Schematic illustration (AI-rendered); shared with the Yield-Threshold and Effective-Stiffness notes; no computed data.*

---

## 2. Extended Thermodynamic Potential & Variational Action

To capture both the classical post-buckling dynamics and the electromechanical back-reaction, the free energy functional per unit area is expanded up to fourth-order invariants in the deflection field $w(\mathbf{x}) \equiv u_z(\mathbf{x})$ and in-plane strain tensor $\varepsilon_{ij}$:

$$
\mathcal{F}[w, u_i, \mathbf{P}] = \int_{\Omega} \left[ \frac{1}{2} C_{ijkl} \varepsilon_{ij} \varepsilon_{kl} + \frac{1}{2} D_0 (\nabla^2 w)^2 - \mu_{ijkl} \left( \partial_k \varepsilon_{ij} \right) P_l + \frac{1}{2 \chi_e} |\mathbf{P}|^2 + \frac{\gamma_{\text{nl}}}{4} (\nabla^2 w)^4 - \mathbf{P} \cdot \mathbf{E}_{\text{ext}} \right] d^2\mathbf{x}
$$

Where:
* $C_{ijkl} = \frac{Y}{1+\nu} \left( \delta_{ik}\delta_{jl} + \frac{\nu}{1-\nu}\delta_{ij}\delta_{kl} \right)$ is the 2D elastic stiffness tensor ($Y \approx 340\,\text{N/m}$, $\nu \approx 0.16$).
* $D_0 \approx 1.2 - 1.6\,\text{eV}$ is the intrinsic bare bending rigidity of uncharged graphene.
* $\mu_{ijkl}$ is the phenomenological flexoelectric tensor coupling strain gradients to dipole moments.
* $\chi_e$ denotes the effective dielectric/vacuum susceptibility of the localized 2D manifold.
* $\gamma_{\text{nl}}$ regulates the quartic geometric stabilization against singular curvature collapse.

### 2.1 Constitutive Flexoelectric Relation

Minimizing $\mathcal{F}$ with respect to the polarization degree of freedom ($\delta \mathcal{F} / \delta \mathbf{P} = 0$) yields the instantaneous constitutive polarization:

$$
P_l = \chi_e \left[ \mu_{ijkl} \left( \partial_k \varepsilon_{ij} \right) + E_{l}^{\text{ext}} \right]
$$

Substituting this stationary relation back into the free energy eliminates $\mathbf{P}$, giving rise to an effective elastic-flexoelectric continuum with renormalized bending and strain-gradient stiffness coefficients.

---

## 3. Modified Non-Linear Föppl–von Kármán (FvK) Formalism

Under finite out-of-plane deflections ($w$), the geometrically non-linear strain tensor assumes the classic von Kármán form:

$$
\varepsilon_{ij} = \frac{1}{2} \left( \partial_i u_j + \partial_j u_i + \partial_i w \partial_j w \right)
$$

The coupled dynamic evolution of the out-of-plane deformation $w(\mathbf{x}, t)$ and the Airy stress function $\Phi(\mathbf{x}, t)$ (where $\sigma_{ij} = \epsilon_{ik}\epsilon_{jl}\partial_k \partial_l \Phi$) incorporates both inertial damping and the flexoelectric polarization back-stress:

$$
\rho_{2\text{D}} \ddot{w} + \eta \dot{w} + D_{\text{eff}}(\kappa) \nabla^4 w - \left( \partial_i \partial_j \Phi \right) \left( \partial_i \partial_j w \right) - \mu_{\text{eff}} \nabla^2 \left( \nabla \cdot \mathbf{P} \right) = \mathcal{S}_{\text{drive}}
$$

$$
\frac{1}{Y} \nabla^4 \Phi = -\frac{1}{2} [\![ w, w ]\!] - \alpha_{\text{flexo}} \nabla^2 \left( \kappa_{xx} \kappa_{yy} - \kappa_{xy}^2 \right)
$$

Here, $[\![ A, B ]\!] \equiv \partial_{xx} A \partial_{yy} B + \partial_{yy} A \partial_{xx} B - 2\partial_{xy} A \partial_{xy} B$ represents the Monge–Ampère bilinear differential operator, while $\mu_{\text{eff}} = \chi_e \mu^2$ reflects the direct self-screening flexoelectric reaction.

---

## 4. The Curvature Threshold ($\kappa_c$) & Regime Shift

A primary assertion of the **CRG-Flux Framework** is that flexoelectric coupling is non-monotonic across topological curvature scales:
        Linear Acoustic Regime           Nonlinear Wrinkling Regime        Yield Shell / Plastic Screening
    |-----------------------------|-----------------------------------|-----------------------------------|
    0                        \kappa_c                             \kappa_{\text{yield}}                  \kappa \to \infty
    (Weak dipolar polarization)     (Spontaneous corrugated cascades)    (Bond reconstruction / B-Fracture)



1. **Sub-Critical Regime ($\kappa < \kappa_c$):**
   * The graphene sheet responds elastically.
   * Dipole formation is strictly linear: $\mathbf{P} \propto \nabla \kappa$.
   * Effective stiffness undergoes minimal renormalization: $D_{\text{eff}} \approx D_0$.

2. **Transition Threshold ($\kappa \sim \kappa_c \equiv \sqrt{\sigma_c / D_0}$):**
   * Transverse acoustic phonons soften dynamically.
   * Spontaneous periodic buckling generates hierarchical wrinkling patterns with characteristic wavelength (valid for $\kappa < \kappa_c / \sqrt{\xi_{\text{flexo}}}$):
     $$
     \lambda_{\text{wrinkle}} \approx 2\pi \left( \frac{D_0}{\sigma_{\text{ext}}} \right)^{1/4} \left[ 1 - \xi_{\text{flexo}} \left( \frac{\kappa}{\kappa_c} \right)^2 \right]^{-1/2}
     $$

3. **Super-Critical / Yielding Regime ($\kappa \ge \kappa_{\text{yield}} \sim \sqrt{\sigma_y / D_0}$ governed by the $\sigma_y / \kappa_c$ threshold switch):**
   * Local in-plane stresses exceed the tensile yield limit $\sigma_y$.
   * Linear flexoelectricity breaks down, triggering dynamic bond reconfiguration (Stone–Wales defects, 5-7 dislocation loops).
   * Energy dissipation transitions into the **Self-Regulating Yield Shell** of the buffer layer.

---

## 5. Connections to Pre-Friedmann Discontinuities & B-Fracture

The corrugated flexoelectric graphene sheet provides the explicit 2D micro-mechanical analogue for macro-boundary behavior in the Pre-Friedmann regime:

* **Analogy of Bound Charges to Crack Boundaries:**
  The 2D bound charge density induced by inhomogeneous curvature:
  $$
  \rho_{\text{bound}} = -\nabla \cdot \mathbf{P}_{\text{flexo}} = -\mu_{\text{eff}} \nabla^2 (\text{Tr}\,\boldsymbol{\kappa})
  $$
  provides a direct mathematical and phenomenology-preserving mapping to the magnetic pole density $\rho_m = -\nabla \cdot \mathbf{M}$ exposed across the discontinuous crack interfaces in permanent magnets (CRG-Flux B-Fracture model).
* **Reactive Energy Regulation:**
  Curvature localization at graphene wrinkles concentrates electric fields ($\mathbf{E} \sim \nabla \rho_{\text{bound}}$), reproducing the **Tip Effect**. This establishes a negative feedback mechanism preventing singular energy collapse through localized electrostatic stiffness softening.

---

## 6. Measured / Predicted Register (E4)

> **Epistemic status:** this note mixes three kinds of quantities. The register below
classifies **every** load-bearing number in §§2–5 as (M) measured, (L) literature-standard,
or (P) predicted by this framework. **No CRG-specific parameter (κ_c, ξ_flexo, κ_yield, γ_nl)
has been measured**; the experimental anchor validates the *existence and curvature
dominance* of the effect, not this framework's parameterization.

| # | Quantity / Claim | Value | Status | Source / Protocol |
|---|---|---|---|---|
| 1 | Flexoelectric polarization at sharp wrinkles | local electrical-potential shift at the sharpest graphene wrinkles (graphene on MoS₂, naturally formed ridges) | **(M) measured** | Iyengar et al., *Adv. Mater.* **2026**, e18224, DOI: [10.1002/adma.202518224](https://doi.org/10.1002/adma.202518224) |
| 2 | Mechanism = quantum **orbital** flexoelectricity | charge redistribution via orbital-overlap change around wrinkle ridges, matching atomic-scale calculations | **(M) measured** (+ atomic-scale theory in-source) | same ref; preprint [arXiv:2503.21996](https://arxiv.org/abs/2503.21996) |
| 3 | Curvature dominance over amplitude | wrinkle **sharpness**, not height, controls the electrical response | **(M) measured** | same ref (Rice Univ. statement, Iyengar quote) |
| 4 | Enhancement magnitude | polarization ≈ **10⁵–10⁷×** larger flexoelectric systems | **(M) measured — order-of-magnitude estimate** (authors' own caveat: smallest bends not atom-resolvable; key quantities model-assisted) | same ref; scope caveat registered |
| 5 | 2D elastic constants: Y ≈ 340 N/m, ν ≈ 0.16 | graphene stiffness tensor input (§2) | **(L) literature-standard** | Y: Lee et al., *Science* **321**, 385 (2008); ν: graphene literature range |
| 6 | Bare bending rigidity D₀ ≈ 1.2–1.6 eV | uncharged-graphene D₀ spread (§2) | **(L) literature range** (theory + experiment spread, not this experiment) | graphene bending-rigidity literature |
| 7 | Curvature threshold κ_c ≡ √(σ_c/D₀) defining the regime shift | §4 normalization | **(P) predicted [model]** — not measured in the experimental normalization | this framework, §4.2 |
| 8 | Three-regime ladder: linear acoustic → wrinkling → Yield Shell | non-monotonic response across κ scales | **(P) predicted [model]** — qualitative support only (row 3 measures curvature dominance, not the ladder) | this framework, §4 |
| 9 | Wrinkle wavelength λ ∝ (D₀/σ_ext)^{1/4} with flexo correction [1 − ξ_flexo(κ/κ_c)²]^{−1/2} | §4.2 scaling | **(P) standard FvK theory + [model] correction** (the ξ_flexo factor is this framework's) | classic wrinkling theory; correction: this framework |
| 10 | Yield activation (Stone–Wales / 5-7 loops) at κ_yield ~ √(σ_y/D₀) | bond reconstruction channel | **(P) predicted [model]** — defect activation under strain is literature-known; the σ_y/κ_c threshold switch is this framework's | this framework, §4.3 |
| 11 | ρ_bound ↔ crack pole-density mapping (B-Fracture) | bound-charge/crack-boundary correspondence | **(P) structural analogy** — explicitly analogy, not derivation | this framework, §5 |
| 12 | Tip-effect negative feedback (E-field concentration prevents singular collapse) | electrostatic softening feedback | **(P) predicted [model]** | this framework, §5 |

**Summary line:** rows 1–4 are the experimental anchor (one paper, one system);
rows 5–6 are standard inputs; rows 7–12 are this framework's [model] content.
A future falsification test is explicit: measure a *calibrated* polarization vs. κ
curve on wrinkle ensembles and check whether the CRG threshold normalization
(row 7) or any competitor fit (plain power law) describes it better.

## 7. Mathematical Cross-References & Vault Links

* [[Tip Effect and Local Curvature Tensor]]: Formulation of the geometric stress enhancement tensor $\mathcal{K}_{ij}$ and curvature singularities.
* [[Yield Threshold]]: Formal derivation of the critical threshold switch $\sigma_y / \kappa_c$ and plastic activation barriers.
* [[Effective Stiffness Reconstruction]]: Full nonlinear renormalization group flow of $D_{\text{eff}}(\kappa, \omega)$.
* [[B-Fracture Analogy & Dynamic Cohesion]]: Mapping of dynamic edge polarization to magnetic crack dipoles and Pre-Friedmann closure boundaries.
* [[Buffer Layer and Non-Equilibrium Transport]]: Dissipative screening mechanisms preventing reactive phase leakage.
