---
title: "Family-Register-Mapping"
created: 2026-09-28
updated: 2026-09-28
author: "Adel Gachkar"
license: "CC-BY-4.0"
zenodo_section: "Index"
status: "canonical"
tags: [Index, Family-Mapping, LIMEN, SPUMA, Register, Tensions]
---

# Family-Register-Mapping — Six CRG-Flux Pillars ↔ LIMEN/SPUMA Registers

> **Epistemic status (read first):** this note registers **structural correspondences
> between frameworks**, not derivations. Every row carries an explicit label in the
> family's own vocabulary: `[structural]` (same logical role in both frameworks),
> `[exact]` (a formula or constant identical on both sides), `[measured]` (executed
> numerical protocol), `[model]` (an identification adopted as a working choice).
> Nothing here transfers a numerical value from one vault into another as a fact;
> nature-side status of all imported constants remains **F3** in the canonical home
> (LIMEN `08_Protocol/Two-Realm-Register`).

## 1. Source registers (canonical homes)

| Framework | Register | Content used here |
|---|---|---|
| LIMEN-VACUI | `08_Protocol/Two-Realm-Register` | work bank W1–W7, W4b, W4c (9 done / 0 pending); silence rows S1–S4; framework-self flags F1–F3; the generative triad constraint × silence × event; norms E0–E5 |
| LIMEN-VACUI | `10_Reference/Emergence-Balance-Reference` + Vault `01_Foundations/Rank-Ladder-Glossary` | emergence as registry event seeded by ΔB; rank ladder scalar → vector → tensor → components → dynamics; energy as scalar ledger and dynamics |
| SPUMA-VACUI | `04_Companion_Mapping/Companion-Bridge` | shared constants (δθ = 7.356103°, φ_max = 0.7405, κ_hop = 0.025 g²ω₀, f_c ≈ 30 THz); mechanism correspondence table; the LIMEN↔SPUMA parameter map (g_max = 0.297, τ_q = 40, κ = 0.03 ⇔ b = 0.285); unified register (negative coupling breaks the p_f floor) |
| SPUMA-VACUI | `02_Constraints/K1-Cavity-Size-Distribution` | b_c = 0.126, p_f = e^{−2bm₀} (κ_fit = 3.17), τ = 2.02–2.03, three regimes + colored-noise fourth |
| CRG-Flux | `00_Index/CRG-Flux_Conceptual_Integration_Analysis` | Pillars I–VI as summarized below |

## 2. The six pillars in one line each

| Pillar | Core content | Registered quantities |
|---|---|---|
| **I — Graphene flexoelectric wrinkling** | C₆/D₆h symmetry breaking by out-of-plane deflection; strain-gradient polarization; pseudo-gauge A_pseudo ∝ ∇²w | P = μ:∇ε; ρ_flexo = −∇·P; **experimental anchor (M):** quantum orbital flexoelectricity at graphene wrinkles — effect existence + curvature (sharpness) dominance measured, enhancement ~10⁵–10⁷× (Iyengar et al., *Adv. Mater.* e18224, 2026, DOI 10.1002/adma.202518224; theory origin Kalinin & Meunier, PRB 77, 033403, 2008). All CRG-specific parameters (κ_c, ξ_flexo, κ_yield, γ_nl) remain `[model]` — full 12-row classification in the note's Measured/Predicted Register (§6) |
| **II — Crack-in-magnet analogy → pre-Friedmann closure** | ∇·B = 0 forbids monopoles; cleavage makes σ_m = M·n̂ pairs; extended action stationary at boundary: δS_ext = 0 | σ_m = −⟦M⟧·n̂; interface charge σ = −⟦Ψ⟧·n̂ with exact dipole conservation ∮σ + ∫ρ = 0 |
| **III — Yield-threshold switching** | dynamic discriminant between elastic storage / active buffer / topological closure | Θ_yield = σ_y/κ_c − Γ_eff(Φ̇); sign convention: > 0 elastic, ≈ 0 buffer, < 0 closed |
| **IV — Nonlinear regime shift (solitonic localization)** | Hookean breakdown at κ_local ~ A/λ² ≥ κ_c; quartic stabilization | F = ½Dκ² + ¼βκ⁴ − μ₁κP − ½χ⁻¹P² + λP²κ² |
| **V — Self-regulating yield shell** | effective stiffness decays toward finite residual baseline; singular screening without divergence | D_eff(r) = D₀[1 − tanh((κ−κ_c)/δ)] + D_res (tanh branch is the canonical form) |
| **VI — B-fracture dynamics + attractor proof** | cohesive traction law + flux coupling; three-variable flow with bounded attractor; Routh–Hurwitz verified at every stable branch (10⁵ draws, zero violations) | uniqueness of the frozen-core branch under the sufficient condition γ₂μ/λ ≤ α₂; bistability outside — stability claim, not global uniqueness |

## 3. Pillar ↔ register mapping table

| CRG-Flux pillar | LIMEN register counterpart | SPUMA register counterpart | Correspondence status | What is shared / what is not |
|---|---|---|---|---|
| **I — flexoelectric polarization P = μ:∇ε** | A3 (arrow from registration): direction-making events; the W4b chiral five-phase register — parity lives in **direction structure**, not magnitude | A3 (edge-polarization wall envelope): polarity **derived** from edge sweeping, not defaulted | `[structural]` — same logical role: local symmetry breaking as the generator of a directed boundary response | Shared: gradient-driven, symmetry-forbidden-in-flat-phase response. Not shared: CRG uses a real strain-gradient tensor of a 2D lattice; LIMEN/SPUMA register a synthetic-gauge phase deficit. No coefficient transfer (μ_ijkl is CRG-local). |
| **II — broken-magnet closure σ = −⟦Ψ⟧·n̂, ∮σ + ∫ρ = 0** | A1 (silent boundary) + K2 (release rings): the boundary does not radiate; what crosses is registered, not emitted | K2 (polarization discontinuity → trapped wall): R_loss → 0, reactive storage — the Companion-Bridge marks this row **exact** ("trapped field = reactive storage") | `[structural]` with one `[exact]` SPUMA row | Shared: zero-net-flux interface + exact compensation identity. Tension T1 (§4): CRG's Ψ jump is a field discontinuity; SPUMA's is a polarization discontinuity — same conservation skeleton, different carrier. |
| **III — Θ_yield = σ_y/κ_c − Γ_eff** | the K1 apparatus: one-sided bias depth d; d_class = 0.0686 (ε = 0.1); classification threshold of the residue test (rel(d) = d/(m+d), m = 0.61722) | K1 freezing edge: b_c = 0.1263 ± 0.0002, p_f = e^{−2bm₀}; three regimes of the size distribution | `[structural]` + `[measured]` on both sides — **this is the closest quantitative touch point in the family** | Shared: a scalar discriminant separates a storing phase from a dissipative/screening phase, with measured thresholds (0.0686 vs 0.126 in their own units; ratio R_edge = 1.841 ± 0.002 is the family's registered universal-decade statement). Not shared: Θ mixes stress/curvature/dissipation-rate in one formula; the K1/LIMEN pair keeps two orthogonal axes (b and d) joined only at the registered encounter point (b, d) = (0.0574, 0.0686). CRG's Θ is **not** a third reading of b_eff — see tension T2. |
| **IV — quartic stabilization, solitonic localization** | no direct row — nearest: the residue test's real-tension branch (R/T₀ = 0.4929, SNR = 892.7: invariant under re-narration = genuinely nonlinear residue) | A4 (intrinsic harmonics from antagonism) + `03_Cavity_Harmonics/Spectral-Regime-Prediction`: single-scale vs power-law spectral regimes | `[structural]`, weakest row — honest gap | Shared: nonlinear self-interaction prevents collapse and creates localized structures. Not shared: CRG's quartic term is geometric (κ⁴); SPUMA's nonlinearity is spectral (cavity harmonics). **No executed protocol links the two nonlinearity channels** — registered as open question OQ-C4-1 (§5). |
| **V — D_eff tanh-softening → D_res** | Balancer-Cushion: the middle-atmosphere cushion absorbs surplus constraint without infinite inflation | Buffer layer (self-regulating transport): dissipative screening; the bad-metal plateau ρ(T) ~ const | `[structural]` — three framings of one anti-divergence function | Shared: a finite residual baseline replaces divergence at the singularity. Distinct implementations: tanh stiffness decay (CRG) / cushion dynamics (LIMEN) / dissipative transport screening (SPUMA). Analogical role alignment per the Emergence-Balance-Reference convention — **analogical, not derivational**. |
| **VI — attractor proof (RH + bounded flow + honest bistability)** | Ward invariance discipline (W7): outputs invariant under re-narration; the invariance-residue test as measure of dissolution vs evasion | K1 first-passage convergence: p_f = e^{−2bm₀} confirmed with κ_fit = 3.17 ± 0.1 vs 2m₀ = 3.0 (5.7% finite-fluctuation correction) | `[structural]` + `[measured]` both sides | Shared: stability/convergence is claimed **only where executed batteries license it**, and E4-corrections are registered when over-claims are caught (CRG: uniqueness → conditional + bistability, mirroring LIMEN's own W1 15.75 → 1.841 correction). This methodological kinship is the deepest family trait. |

## 4. Tensions — registered, not buried (E4 discipline)

| # | Tension | Sides | Registered resolution path |
|---|---|---|---|
| **T1** | Carrier mismatch at the closure interface: CRG closes with a **field jump** ⟦Ψ⟧ on a fracture line (2D electrostatics); SPUMA closes with a **polarization jump** on a wall envelope; LIMEN closes with **registration** (one-way absorbing silence). Three closure operators, one conservation skeleton | II ↔ K2 ↔ A1/K2-LIMEN | Keep all three as distinct specializations of the zero-net-flux constraint; any unification needs a shared operator — candidate: the Laplacian coupling κ of the LIMEN–SPUMA bridge (R(κ) → 1 is the registered iid limit). Open. |
| **T2** | Threshold-composition optimism: the temptation to read Θ_yield as a composite of b + d (the unified-register axis b_eff = b + d). The W2 verdict forbids this: at the encounter point the spectrum is the plain critical one — composition is **spectrally invisible**; the gauge identity mask(b,d) = mask(b+d,0) makes any composite reading untestable on the critical axis | III ↔ W2 (LIMEN) | CRG's Θ stays a **standalone discriminant** with its own measured constants (σ_y, κ_c, Γ₀, Φ̇_c); it is not mapped onto (b, d) space. If CRG ever joins the W4c gate, it enters as an independent dataset candidate, not as a re-labeling. |
| **T3** | Vocabulary collision on "phase": CRG "phase" = thermodynamic/mechanical regime; LIMEN "phase" = pre/post-boundary register epoch; SPUMA "phase" = wave/harmonic phase (the phase-debt oscillator). Three homonyms in one family | all | All cross-references must say which "phase" (regime-phase, epoch-phase, wave-phase). This note uses **regime-phase** for Pillars III–V and **wave-phase** only inside pillar I's pseudo-gauge context. |
| **T4** | Uniqueness vs bistability asymmetry: CRG registered that stable equilibria can be **multiple** (bistability measured at 0.37% of parameter space — W8 re-measurement); the unified register's exclusive identity p_U = p_A + p_B holds at machine precision — two frameworks with different multiplicity structure at their fixed points | VI ↔ Unified-Register-Integration (LIMEN) | **RESOLVED by W8 (2026-09-28):** the multiplicity-aware test was executed — a bistable CRG parameter set maps to a DEFINITE exit structure: the two stable branches split the two exits (melted → SPUMA freeze-out, frozen → LIMEN registration), calibration-robust 0/9. The identification "CRG attractor = LIMEN exit" now has a measured, multiplicity-aware answer; the remaining open layer is only the [model] status of the seed map itself (OQ-C4-2b sensitivity ladder). |
| **T5** | Standing prohibitions hold unchanged: LIMEN S1–S4 (pre-boundary silence, first cause, constant values, absolute energy) apply to CRG's pre-Friedmann language too — the CRG "pre-Friedmann ground state" is a **boundary-side** construct (stationary action on M with boundary terms), not a statement about the pre-boundary | II ↔ S1/S2 | Recorded so no reader imports CRG's pre-Friedmann manifold as a picture of LIMEN's pre-boundary. The sanctity clause (family contract, SPUMA Companion-Bridge §3b) is inherited verbatim. |

## 5. Open questions created by this mapping (work-realm candidates)

| # | Question | Conceivable tool | Status |
|---|---|---|---|
| OQ-C4-1 | Does the CRG quartic stabilization (Pillar IV) and the SPUMA harmonic antagonism (A4) belong to one nonlinearity class? | a shared variational benchmark: fit both to one curvature-localization profile and compare residual structure | `[bank: pending]` — no protocol executed |
| OQ-C4-2 | Does a bistable CRG parameter set (the ~2% region outside the sufficient condition) map to a definite exit of the LIMEN unified register? | run the CRG battery at bistable points, feed each stable branch's x* as LIMEN seed density, read the exit channel | **✅ EXECUTED 2026-09-28 — YES, the two stable branches SPLIT the two exits.** Tool: LIMEN `tools/limen_w8_crg_branch_register.py` (output `tools/limen_w8_crg_output.txt`). The recorded exemplar reproduces exactly [exact] (x* = 0.0029 stable / 0.0994 saddle / 0.9449 stable). The low-x (melted-core) branch is dominantly read by the SPUMA freeze-out exit B (B-solo 0.4022 vs A-solo 0.3153); the high-x (frozen-core) branch by the LIMEN registration exit A (A-solo 0.3391 vs B-solo 0.2302) [measured on the registered [model] density-preserving map]; 0/9 calibration flips across the (eta, delta) grid. **Reading: CRG bistability maps onto the register's silence-vs-registration duality — melted core ↔ SPUMA freeze-out, frozen core ↔ LIMEN registration.** Frequency re-measurement [exact, 20k draws]: multi-root 3.02% of outside-condition draws, bistable **0.37%** (74/20000) — E4 refinement of the earlier "~2% bistable" phrasing: multi-root is ~3%, true bistability ~0.4%, and "on average two stable equilibria per multi-root draw" is refuted (mean 1.25). Migration registered in the LIMEN Two-Realm-Register as row **W8** (bank 10/0). |
| OQ-C4-3 | Is the tanh softening of D_eff (Pillar V) and the LIMEN cushion's absorbing profile the same fixed-point structure? | compare relaxation spectra of both linearized operators | `[bank: pending]` |

These three rows enter the work bank only after a protocol is executed; until then
they are collateralized questions, not claims (Two-Realm-Register migration rule).

## 6. Contact points — summary scorecard

| Contact | Strength | Label |
|---|---|---|
| Threshold discriminants (Θ_yield ↔ d_class/b_c) | strongest — both sides measured, one registered ratio (R_edge = 1.841 ± 0.002) in the same decade | `[structural]` + `[measured]` |
| Anti-divergence trio (tanh / cushion / buffer) | strong — one function, three implementations | `[structural]` |
| Closure conservation (∮σ + ∫ρ = 0 ↔ R_loss→0 ↔ registration) | strong skeleton, carrier mismatch registered (T1) | `[structural]` |
| E4 self-correction culture (uniqueness→bistability ↔ 15.75→1.841) | methodological, family-defining | `[protocol-mirror]` |
| Nonlinearity channels (quartic vs harmonics) | weakest — no executed link (OQ-C4-1) | `[bank: pending]` |

## 7. Related

- [[MOC - CRG-Flux Architecture]] — the map
- [[CRG-Flux_Conceptual_Integration_Analysis]] — the six pillars in full
- [[Figure-and-Asset-Register]] — provenance record
- Family canonicals: LIMEN-VACUI `08_Protocol/Two-Realm-Register`, `07_Companion_Mapping/Companion-Bridge`, `10_Reference/Emergence-Balance-Reference`; SPUMA-VACUI `04_Companion_Mapping/Companion-Bridge`, `02_Constraints/K1-Cavity-Size-Distribution` (cross-repository pointers, not local copies)
