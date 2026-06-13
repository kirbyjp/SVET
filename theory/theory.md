---
title: "Static Vacuum Excitation Theory (SVET)"
subtitle: "A capacity-limited Planck-scale physical vacuum as a unified foundation for General Relativity and Quantum Gravity"
author: 
  - John Kirby
date: "June 2026"
abstract: |
  This document presents Static Vacuum Excitation Theory (SVET), a discrete resource-accounting model of the physical vacuum. SVET models the vacuum as a network of Planck-scale nodes with finite update budgets and local update rules. From these primitives we derive emergent wave mechanics, a divergence-free account of quantum excitations, finite-core black holes, and a cadence-based mapping to gravitational phenomena. The framework is written as a living Markdown document (MathJax/LaTeX compatible) intended for iterative development, Pandoc conversion, and eventual arXiv/journal submission.
keywords: [Quantum Gravity, General Relativity, Substrate Physics, Discrete Vacuum, Singularities, CaBS]
geometry: margin=1in
fontsize: 11pt
header-includes:
  - \usepackage{amsmath}
---

# Static Vacuum Excitation Theory (SVET)  
### A capacity‑limited Planck‑scale physical vacuum as a unified foundation for GR and QG

---

## 0. Notes on this document
*This file is the living source for SVET. It is Markdown + MathJax (LaTeX math) and is intended to be converted to LaTeX/PDF via Pandoc for arXiv or journal submission. Use the Git history for versioning; keep the filename `theory.md` as the single source of truth.*

---

## 1. Introduction

*TODO: Describe the motivation for SVET — resolving GR singularities and QFT divergences through a finite substrate. Provide a concise roadmap of the paper and summarize the main claims and predictions.*

---

## 2. Ontology of the Vacuum

### 2.1 The Planck‑Scale Physical Vacuum
*TODO: Define the vacuum as a capacity‑limited, rule‑governed entity. Explain why we treat the vacuum as a network of nodes rather than a continuous field.*

### 2.2 Minimal Local Rules and Assumptions
*TODO: List the minimal rule set governing local updates (causality, adjacency, budget accounting, update resolution order). State assumptions and scope.*

### 2.3 The Node State Bundle
- **B** — capacity (node budget)  
- **S** — strain (current load)  
- **B₀** — baseline capacity (resting budget)  
- **τ₀** — base tick (substrate fundamental tick)  
- **τ_eff** — effective cadence (local update delay)  
*TODO: Define units, ranges, and physical interpretation for each variable. Provide canonical initial conditions and normalization conventions.*

### 2.4 Directional Phase Encoding
*TODO: Explain how orientation of coherent update demand encodes phase information without invoking complex amplitudes. Provide a minimal example showing phase shift via cadence delay.*

### 2.5 Dual‑Channel Propagation
*TODO: Define the coherent (pattern‑preserving) channel and the incoherent (heat/ledger) channel. Explain how energy/exaction partitions between them and how this implements decoherence.*
### 2.7 Incoherent Channel (H) — Definition and Manifestations

**Statement (SVET):**  
In SVET, **H** denotes *incoherent energy* — energy that has left the coherent propagation channel and no longer carries directional phase information. Heat is one possible macroscopic manifestation of H, but H is a substrate‑level category that can produce multiple physical outcomes depending on the local material and boundary physics.

**Definition:**  
- **H (incoherent flux)** = coherent flux that has lost directional consistency due to cadence mismatch, strain overload, budget exhaustion, or internal scattering.  
- Formally, a coherence → incoherence transition occurs when the local load and cadence demand exceed adjacency’s capacity to maintain phase alignment:


\[
\text{If}\quad \text{Strain} \; \lor \; \text{CaBS demand} \;>\; \text{Adjacency coherence capacity} \quad\Rightarrow\quad \text{Coherent}\;\to\;\text{Incoherent (H)}
\]


**Possible macroscopic manifestations of H:**  
- **Thermal phonons (heating)** — incoherent energy couples to lattice vibrations.  
- **Photochemistry / UV curing** — incoherent energy drives chemical bond rearrangements.  
- **Fluorescence / radiative decay** — incoherent excitations re‑emit photons at shifted energies.  
- **Photoelectric emission** — incoherent energy ejects electrons from material.  
- **Structural failure (plastic deformation, fracture)** — coherent stress patterns collapse into incoherent modes that manifest as mechanical damage.  
- **Other sinks** — any process that accepts incoherent energy (e.g., metastable trapping, nonradiative decay).

**Why this distinction matters (SVET advantages):**  
- **Unified mechanism:** Optical decoherence, heating, chemical reactions, and mechanical failure are all instances of the same substrate event: loss of coherence.  
- **Predictive accounting:** CaBS ledger predicts how much energy remains coherent vs. how much becomes H; the material determines the sink.  
- **Falsifiable signatures:** The partitioning ratio (coherent : incoherent) at interfaces and under pump conditions yields measurable predictions (e.g., reflected fraction, fluorescence yield, temperature rise).

**Practical mapping for experiments and simulations:**  
- Track **coherent flux** and **H accumulation** separately in simulations.  
- Report H as an energy flux into the incoherent channel; then map H to specific observables using material response models (phonon coupling constants, cross sections for photoemission, reaction rates, etc.).  
- Use pump‑probe and calorimetric experiments to measure the coherent/incoherent partition and validate CaBS predictions.

**Suggested placement in theory.md:**  
- Add this subsection as **2.7** (Ontology) and cross‑reference in Sections **4 (Flux Algebra)**, **5 (Emergent Wave Mechanics)**, **10 (Material Response & Dispersion)**, and **12 (Predictions)**.  
- Use the phrase **“H = incoherent (decohered) flux”** consistently throughout the document; reserve the word “heat” for specific thermodynamic outcomes of H.

**Concise summary line (for tables/Excel):**  
`H = incoherent flux (decohered energy); heat is one manifestation; other sinks include photochemistry, fluorescence, photoelectric emission, and mechanical failure.`

---

## 3. Capacity Limits and Divergence‑Free Behavior

### 3.1 Finite Excitation Capacity (η_max)
*TODO: Define the maximum excitation per node and how it constrains local field amplitudes.*

### 3.2 Finite Update Cadence (τ_eff)
*TODO: Provide the functional form of cadence slowdown, e.g.:*
$$
\tau_{\text{eff}} = \tau_0\left(1 + \left(\frac{S}{B}\right)^\beta\right)
$$
*TODO: Explain parameter β and physical consequences.*

### 3.3 Why Divergences Cannot Occur
*TODO: Demonstrate how UV divergences are prevented by hard capacity limits and discrete update accounting. Provide a sketch proof or argument.*

### 3.4 Critical Threshold & Phase Transition ⭐
*TODO: Define the critical threshold (the "Redline") where \(B \to 0\). Describe the substrate phase transition (e.g., pair production, reconfiguration) that replaces singular behavior. Relate to Schwinger pair production qualitatively and quantitatively where possible.*

---

## 4. Flux Algebra

### 4.1 Flux as Directional Coherent Update Demand
*TODO: Provide the SVET definition of flux: the directional component of coherent exaction attempting to propagate across adjacency. Clarify notation and units.*

### 4.2 Flux Addition and Cancellation
*TODO: Formalize vector addition rules for flux, including cancellation, superposition, and normalization constraints.*

### 4.3 Propagation, Reflection, and Refraction
*TODO: State local update rules that produce propagation, reflection, and refraction. Include boundary interaction rules and examples.*

### 4.4 The Substrate Ledger (Conservation of Exaction) ⭐
**Statement:** Conservation is a bookkeeping identity of the node update: the outgoing coherent portion, reflected portion, and dissipated heat sum to the node's available exaction.  
$$
R + T + H = 100\%
$$
*TODO: Derive this identity from the node update algorithm and show how it enforces global conservation without invoking a separate conservation law.*

---

## 5. Emergent Wave Mechanics

### 5.1 Local Update → Discrete Wave Equation
*TODO: Derive the discrete wave equation that emerges from repeated local updates. Provide the continuum limit and show correspondence to standard wave PDEs.*

### 5.2 Interference from Vector Superposition
*TODO: Show how interference patterns arise from vector superposition of flux orientations and cadence delays. Provide the double‑slit toy model.*

### 5.3 Dispersion Relations
*TODO: Derive dispersion relations and define the effective refractive index \(n_{\text{SVET}}(\omega)\). Provide low‑frequency and high‑frequency asymptotics.*

---

## 6. Hilbert‑Space Correspondence

### 6.1 Coherence ↔ Amplitude
*TODO: Map coherent pattern amplitude to quantum amplitude analogs.*

### 6.2 Flux Orientation ↔ Phase
*TODO: Show how orientation and cadence produce phase behavior equivalent to complex phase factors.*

### 6.3 Node Ledger ↔ Probability Density
*TODO: Explain how the node ledger and normalized flux distributions correspond to probability densities in measurement statistics.*

### 6.4 Decoherence ↔ Heat Channel
*TODO: Formalize decoherence as irreversible transfer from coherent channel to heat channel and derive decoherence timescales.*

### 6.5 Eigenmodes and Pattern Persistence
*TODO: Define eigenmodes of the substrate and conditions for long‑lived patterns (quasi‑particles).*

---

## 7. QFT Correspondence Layer

### 7.1 Fields as Statistical Summaries
*TODO: Explain how continuum fields arise as statistical summaries of node states over coarse‑grained volumes.*

### 7.2 Excitations as Coherent Flux Packets
*TODO: Define particle‑like excitations as localized coherent flux packets and discuss dispersion, group velocity, and stability.*

### 7.3 Mass as Cadence Penalty
*TODO: Present the mapping where effective inertial mass emerges from cadence penalties or local budget taxation.*

### 7.4 Interactions as Local Strain Coupling
*TODO: Show how interactions arise from local strain coupling and budget negotiation between overlapping patterns.*

### 7.5 Why Renormalization Disappears
*TODO: Argue that renormalization is unnecessary because the substrate enforces finite cutoffs and capacity limits; provide examples.*

---

## 8. GR Correspondence Layer

### 8.1 Curvature as Cadence Gradient
*TODO: Define the mapping between metric curvature and spatial gradients in \(\tau_{\text{eff}}(x)\). Provide leading‑order correspondence.*

### 8.2 Geodesics as Least‑Delay Paths
*TODO: Show that particle trajectories follow least‑delay (least‑cadence) paths and derive the geodesic equation analog.*

### 8.3 Horizons as Capacity Boundaries
*TODO: Define horizons as surfaces where \(\tau_{\text{eff}} \to \infty\) or where coherent propagation is effectively halted.*

### 8.4 Finite‑Core Black Holes
*TODO: Describe finite‑core black hole structure, internal state, and how singularities are replaced by high‑strain cores.*

### 8.5 Hill vs Hole Duality ⭐
*TODO: Present the Hill vs Hole duality: GR's negative potential well vs SVET's positive excitation hill. Show how weak‑field observables coincide while mechanisms differ.*

---

## 9. Causal Boundaries

### 9.1 Maximum Update Rate
*TODO: Define the substrate's maximum update rate and its role in setting a maximum signal speed.*

### 9.2 Adjacency‑Limited Propagation
*TODO: Formalize adjacency hop limits and their effect on causal structure.*

### 9.3 Emergent Lorentz Symmetry
*TODO: Provide arguments and calculations showing how Lorentz symmetry emerges in the long‑wavelength limit from cadence and adjacency constraints.*

---

## 10. Measurement and Decoherence

### 10.1 Detectors as Active Strain Injectors
*TODO: Model detectors as active nodes that inject strain and alter local budgets during measurement.*

### 10.2 Measurement as Cadence Disruption
*TODO: Explain measurement as a cadence disruption that forces coherent patterns into the heat channel.*

### 10.3 Collapse as Loss of Directional Coherence
*TODO: Provide a mechanical description of collapse as irreversible loss of directional coherence and show how statistics reproduce Born‑like rules.*

---

## 11. Material Response & Dispersion

### 11.1 Effective Index \(n_{\text{SVET}}(\omega)\)
*TODO: Define and derive the effective refractive index as a function of local state variables.*

### 11.2 Absorption and Attenuation (μ)
*TODO: Derive attenuation laws and connect to the Beer‑Lambert statistical limit.*

### 11.3 Conductivity and Loss Tangent
*TODO: Map substrate parameters to effective conductivity and loss tangent for engineering analogies.*

### 11.4 Nonlinear Response
*TODO: Describe nonlinear effects (Kerr‑like, saturable absorption) arising from budget saturation.*

### 11.5 Reflection as Accounting Shock ⭐
*TODO: Derive Fresnel‑like reflection from budget rejection at interfaces; show how reflected fraction follows from ledger constraints.*

---

## 12. Computational Implementation Layer

### 12.1 3D‑Native Adjacency (6‑Vector Flux)
*TODO: Specify adjacency topology, indexing, and data structures for 3D simulations.*

### 12.2 The v0.20.4 Flux Engine Logic
*TODO: Document the engine's update loop, resolution order, and pseudo‑code for flux resolution.*

### 12.3 Boundary Conditions and Heat Channel
*TODO: Define boundary conditions used in simulations and the implementation of the heat sink.*

### 12.4 Numerical Stability and Convergence
*TODO: Provide notes on timestep selection, stability criteria, and convergence tests.*

---

## 13. Predictions and Falsifiable Tests

### 13.1 Pump‑Induced Refractive Index Shifts
*TODO: Quantify predicted index shifts under intense pumping and propose pump‑probe experimental setups.*

### 13.2 Finite‑Core Black Hole Signatures
*TODO: List observational signatures (e.g., modified ringdown, core emission spectra) that distinguish finite‑core black holes from classical singularities.*

### 13.3 Cadence‑Based Lensing Deviations
*TODO: Predict small deviations from GR lensing due to cadence gradients and propose observational tests.*

### 13.4 SVET‑Specific Dispersion Curves
*TODO: Provide dispersion curves for SVET and compare to standard QFT/GR expectations.*

### 13.5 Decoherence‑Rate Predictions
*TODO: Provide quantitative decoherence rates for mesoscopic systems and suggest laboratory tests.*

---

## 14. Emergent Continuum

### 14.1 Long‑Wavelength Limit
*TODO: Show how continuum PDEs (e.g., wave equation, Einstein equations in weak field) emerge from coarse‑graining.*

### 14.2 Rotational Symmetry Emergence
*TODO: Demonstrate how rotational invariance appears statistically from isotropic update rules.*

### 14.3 Continuum PDE Recovery
*TODO: Provide explicit derivations for continuum PDE recovery and identify correction terms.*

---

## 15. Correspondence With Observables

### 15.1 Gravitational Redshift and Time Dilation
*TODO: Show that for weak potentials SVET reproduces the Schwarzschild temporal component to leading order.*

### 15.2 Beer‑Lambert Attenuation Limit
*TODO: Reference simulation results demonstrating exponential attenuation as a statistical limit of discrete budget clipping.*

### 15.3 Snell’s Law and Refraction
*TODO: Demonstrate bending from cadence gradients across interfaces and show correspondence to Snell's law in the continuum limit.*

### 15.4 The Schwinger Limit and Critical Field
*TODO: Align the substrate critical threshold with known vacuum pair production thresholds and discuss experimental implications.*

---

## 16. Open Questions and Future Work

### 16.1 Multi‑Particle Interaction and Interference
*TODO: Explore how overlapping exaction patterns negotiate shared budgets and produce many‑body quantum statistics.*

### 16.2 3D Substrate Scaling and Performance
*TODO: Roadmap for scaling simulations from toy 2D sheets to full 3D volumes; computational resource estimates.*

### 16.3 Calibration Against Observational Data
*TODO: Plan for calibrating substrate constants (\(\eta_{\max}\), \(\Phi_0\), \(\tau_0\), \(\beta\)) using LIGO, collider, and astrophysical data.*

### 16.4 Extensions and Alternative Topologies
*TODO: Consider alternative adjacency topologies, anisotropic rules, and coupling to matter fields.*

---

## References

1. Kirby, J. (2026). *Static Vacuum Excitation Theory (SVET) — Project Archive.* (SVET repository and internal notes).  
2. Schwinger, J. (1951). *On Gauge Invariance and Vacuum Polarization.* Physical Review.  
3. Misner, C. W., Thorne, K. S., & Wheeler, J. A. (1973). *Gravitation.* W. H. Freeman.  
4. Peskin, M. E., & Schroeder, D. V. (1995). *An Introduction to Quantum Field Theory.* Addison‑Wesley.  
5. Additional references to be added as sections are completed (arXiv papers, experimental reports, simulation papers).

*TODO: Convert references to BibTeX for Pandoc/LaTeX export and expand to include all cited works.*

---

## Appendices

### Appendix A: Mathematical Derivations
*TODO: Full derivations referenced in the main text, including discrete → continuum limits, ledger algebra proofs, and the derivation of the discrete wave equation.*

### Appendix B: SVET v1.0 Node Specification
*TODO: Authoritative reference for the primary gauges (B, S, B₀, τ) and the processing logic (update order, flux resolution, heat accounting). Include canonical parameter values used in simulations.*

### Appendix C: Forensic Tool Manifest
*TODO: Checksums, version tags, and usage notes for v0.17.1 and v0.20.4 truth toys and flux engines. Include reproducible run instructions and sample outputs.*

### Appendix D: Notation and Conventions
*TODO: Table of symbols, units, index conventions, and shorthand used throughout the document.*

---

© 2026 John Kirby. Licensed under the MIT License.
