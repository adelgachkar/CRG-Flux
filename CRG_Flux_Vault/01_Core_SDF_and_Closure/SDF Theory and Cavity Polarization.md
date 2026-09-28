---
title: "SDF Theory and Cavity Polarization"
created: 2026-09-25
updated: 2026-09-28
author: "Adel Gachkar"
license: "CC-BY-4.0"
zenodo_section: "Core-SDF-and-Closure"
status: "canonical"
tags: [Core, SDF, Cavity-Polarization, Pentagonal-Defect, Screening]
---

# SDF Theory and Cavity Polarization

## 1. Cavity Polarization and Topological Enclosure

In the Structured Defect Framework (SDF), a microscopic cavity (void) of volume $V_c$ bounded by $\partial V_c$ acts as a resonant topological boundary. The presence of non-zero out-of-plane corrugations induces both strain gradients and boundary dipole accumulation.

The net induced cavity dipole moment $\mathbf{P}_{\text{cavity}}$ is evaluated via the boundary flux:
$$\mathbf{P}_{\text{cavity}} = \oint_{\partial V_c} \mathbf{r} \left[ \left( \chi_{\text{eff}} \mathbf{E}_{\text{vac}} + \boldsymbol{\mu}_{\text{flexo}} : \nabla \mathbf{u} \right) \cdot \hat{\mathbf{n}} \right] dS$$

where:
- $\mathbf{r}$ is the position vector along the cavity boundary $\partial V_c$.
- $\hat{\mathbf{n}}$ is the outward surface unit normal.
- $\mathbf{u}(\mathbf{r})$ is the in-plane and out-of-plane displacement field.
- $\boldsymbol{\mu}_{\text{flexo}}$ is the fourth-rank flexoelectric coupling tensor.
- $\chi_{\text{eff}} \mathbf{E}_{\text{vac}}$ represents the vacuum polarization response under boundary curvature constraints.

![Cavity void polarization — boundary flux and screening envelope](../Assets/fig_void_polarization.png)
*Figure 1 — Schematic of inward polarization flux at the cavity boundary $\partial V_c$: bound charge suppresses high-frequency radiative leakage and screens the inner domain. Schematic illustration (AI-rendered); no computed data.*

The inward polarization flux generates an effective boundary charge that suppresses high-frequency radiative leakage, screening the inner domain from outward metric dissipation.

---

## 2. Five-Edge Coupling Hamiltonian

The discrete symmetry of a pentagonal boundary defect (responsible for positive intrinsic disclination and cone formation) is described by an effective 5-edge Hamiltonian:

$$\mathcal{H}_{\text{edge}} = \sum_{k=1}^{5} \left[ -J_{k,k+1} \cos(\theta_k - \theta_{k+1}) + \lambda_5 \cos(5\theta_k) \right] + \mathcal{H}_{\text{field}}[\mathbf{\Psi}]$$

where:
- $\theta_k$ is the local phase angle of the order parameter at boundary edge $k$ (with cyclic boundary conditions $\theta_6 \equiv \theta_1$).
- $J_{k,k+1} > 0$ represents the exchange cohesion between adjacent edges.
- $\lambda_5$ denotes the discrete 5-fold topological locking potential enforcing pentagonal disclination.
- $\mathcal{H}_{\text{field}}[\mathbf{\Psi}]$ governs the static background field interaction:
$$\mathcal{H}_{\text{field}}[\mathbf{\Psi}] = \int_{V_c} \left[ \frac{1}{2} |\nabla \mathbf{\Psi}|^2 + \frac{1}{2} m_{\text{eff}}^2 |\mathbf{\Psi}|^2 \right] d^2r$$

Dissipative leakage from the cavity to the surrounding bulk lattice is captured dynamically via the Rayleigh dissipation function:
$$\mathcal{R}_{\text{leak}} = \frac{1}{2} \xi \int_{V_c} \left| \frac{\partial \mathbf{\Psi}}{\partial t} \right|^2 d^2r$$
where $\xi > 0$ is the non-equilibrium leakage damping coefficient.

---

## 3. Nonlinear Field Screening and Metastable Equilibrium

Stationary minimization of the action $\delta S_{\text{SDF}} = 0$ in the presence of self-interaction yields the nonlinear screening equation for the envelope field $\mathbf{\Psi}(\mathbf{r})$:

$$\nabla^2 \mathbf{\Psi} - m_{\text{eff}}^2 \mathbf{\Psi} = \beta |\mathbf{\Psi}|^2 \mathbf{\Psi}$$

where:
- $m_{\text{eff}}$ is the effective screening mass induced by the flexoelectric gap.
- $\beta > 0$ characterizes repulsive cubic nonlinearity preventing catastrophic field collapse.

In cylindrical coordinates $(r, \phi)$, the symmetric solution exhibits rapid exponential decay away from the boundary wall:
$$\mathbf{\Psi}(r) \sim \mathbf{\Psi}_0 \frac{e^{-m_{\text{eff}} (r - R_c)}}{\sqrt{r}}, \quad r > R_c$$

This rapid attenuation confines topological stress strictly inside the buffer zone, establishing the non-singular foundation of the pre-Friedmann ground state.

---

## 4. Architectural Links
- [[MOC - CRG-Flux Architecture]]
- [[Pre-Friedmann Ground State & Action]]
- [[B-Fracture Analogy & Dynamic Cohesion]]
- [[Coupled Dynamical Equations]]
