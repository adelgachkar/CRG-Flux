---
title: "Figure-and-Asset-Register"
created: 2026-09-28
updated: 2026-09-28
author: "Adel Gachkar"
license: "CC-BY-4.0"
zenodo_section: "Index"
status: "canonical"
tags: [Index, Figures, Assets, Provenance, Register]
---

# Figure-and-Asset-Register

> **Purpose (audit closure, 2026-09-28):** the technical audit scored this vault
> 9.0/10 with a residual 0.5 for "decorative figures without data captions and the
> unidentified `conf239-1.pdf`". This register resolves both: every visual asset is
> now embedded in exactly one canonical note with an honest caption (schematic /
> AI-rendered / no computed data), and every PDF has verified bibliographic
> provenance. All 18 notes now carry complete frontmatter (tags included) and all
> 10 embeds use correct relative paths.

## 1. Figures (8) — embed status and honest caption policy

| Asset | Size | Canonical host note | Status before → after |
|---|---|---|---|
| `fig_cosmology_potential_curve.png` | 1.5 MB | 01_Core_SDF_and_Closure/Pre-Friedmann Ground State & Action | bare embed → **captioned, relative path fixed** |
| `fig_void_polarization.png` | 204 KB | 01_Core_SDF_and_Closure/SDF Theory and Cavity Polarization; shared in 06 (KPZ) | captioned inline → standardized |
| `fig_curved_lattice_charge.png` | 30 KB | 02 (Quantum Flexoelectricity); shared in 03 (Yield) & 04 (Stiffness) | bare embeds → **captions with cross-note sharing note** |
| `fig_tip_field_enhancement.png` | 1.4 MB | 03_Geometric_Singularity_Tip/Tip Effect and Local Curvature Tensor | captioned → standardized |
| `fig_broken_magnet_analogy.png` | 167 KB | 04_Buffer_and_B_Fracture/B-Fracture Analogy & Dynamic Cohesion | captioned inline → standardized |
| `fig_phase_portrait_attractor.png` | 1.4 MB | 05_Phase_Space_Attractor/Coupled Dynamical Equations | bare embed → **captioned (schematic, no simulated trajectories)** |
| `fig_mesoscopic_iv_curve.png` | 25 KB | 06_Foundational_Literature/Mesoscopic Transport and Green Functions | bare embed → **captioned (not a reproduction of Wang–Wang–Guo data)** |
| `fig_three_layer_framework.png` | 2.1 MB | 05_Phase_Space_Attractor/Three-Layered Dynamical Framework | **was orphaned (zero embeds) → now installed** with explicit "decorative companion to the mermaid graph" disclaimer |

**Caption policy (honesty discipline):** every caption states (a) what is shown,
(b) the governing formula it illustrates, and (c) an explicit
"AI-rendered schematic — no computed data" disclaimer. No figure in this vault is
presented as simulation output or experimental data; the only measured sources are
the four literature PDFs below.

## 2. PDF assets (4) — verified provenance

| File | Identified as | Verification |
|---|---|---|
| `9902307v1.pdf` (306 KB) | **arXiv:cond-mat/9902307** — B. Wang, J. Wang & H. Guo, "Nonlinear I-V Characteristics of a Mesoscopic Conductor" (1999) | first-page text extraction |
| `1912.02126v2.pdf` (1.3 MB) | **arXiv:1912.02126** — M. Patmiou & V. G. Karpov, "Qualitative methods in condensed matter physics" (2019) | first-page text extraction |
| `2505.02591v1.pdf` (100 KB) | **arXiv:2505.02591** — A. B. Balakin & A. O. Efremova, "Extended Einstein-Dirac-aether theory: Spinor modifications of the dynamic aether kinetic term" (2025) | first-page text extraction; source note rebuilt from this abstract |
| `conf239-1.pdf` (10.9 MB, 74 pp.) | **Kazumasa A. Takeuchi (Univ. Tokyo), "Introduction to the KPZ equation and its experimental aspects" — Lecture notes, Les Houches School on KPZ, ver. 3** | embedded PDF metadata (Title/Author) + first-page text |

**`conf239-1.pdf` provenance note:** the filename is a conference-management
download artifact with no semantic content. Identity was recovered from the file's
own embedded metadata (Title: *"Interface Growth with Noise: experiments and
theory"*, Author: 竹内一将 = Kazumasa A. Takeuchi; Creator: PowerPoint PDFMaker 17,
July 2024). **SHA-256 (first 16 hex): `c71a4208b458d409`.** It is the primary
pedagogical/experimental anchor of the note *KPZ Growth and Surface Fluctuations*,
where it is now formally cited.

## 3. Embed hygiene

- 10/10 image embeds now use **correct relative paths** (`../Assets/…` from
  subfolder notes — the bare `![[Assets/…]]` form only resolves when the note sits
  at the vault root, which broke 5 embeds).
- Every figure has exactly one canonical host + explicitly-marked shares
  (`fig_void_polarization.png` ×2, `fig_curved_lattice_charge.png` ×3).
- Zero orphaned images after installing `fig_three_layer_framework.png`.
- Obsidian double-bracket math jumps (`$⟦Ψ⟧`-style) were previously converted to
  `\llbracket/\rrbracket` so the wikilink parser ignores them; verified again in QA.

## 4. Related

- [[MOC - CRG-Flux Architecture]]
- [[CRG-Flux_Conceptual_Integration_Analysis]]
