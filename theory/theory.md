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
### Preface: Etymological Context
The acronym SVET (Static Vacuum Excitation Theory) also mirrors the word for "world" and "light" in several European languages. This dual meaning reflects the model’s purpose: to describe the fundamental structure of the cosmos (the world) and the propagation of coherent excitations (light) through a unified, capacity-limited node network.

### 1.1 What the Node Network Is
The node network is the vacuum—the same vacuum studied in quantum field theory, cosmology, and high-energy physics. SVET does not introduce an additional medium; it reinterprets the existing vacuum as a static network of update sites whose localized, discrete excitations manifest as physical patterns.

The vacuum node network supports waves rather than point-like particles. What experimental physics registers as “particles” are localized, self-maintaining coherence-patterns whose tightly confined structure produces particle-like behavior.

*TODO: Describe the motivation for SVET — resolving GR singularities and QFT divergences through a finite substrate. Provide a concise roadmap of the paper and summarize the main claims and predictions.*

---

## 2. Ontology of the Vacuum
### 2.0 Ontology of the Vacuum
The node network is the vacuum—the same vacuum studied in quantum field theory, cosmology, and high-energy physics. SVET does not introduce an additional medium; it reinterprets the existing vacuum as a static network of update sites whose localized, discrete excitations manifest as physical patterns.

The vacuum node network supports waves rather than point-like particles. What experimental physics registers as “particles” are localized, self-maintaining coherence-patterns whose tightly confined structure produces particle-like behavior.

### 2.1 The Planck‑Scale Physical Vacuum
*TODO: Define the vacuum as a capacity‑limited, rule‑governed entity. Explain why we treat the vacuum as a network of nodes rather than a continuous field.*

### 2.1 Patterns as Particles
Within the node network, physical entities are not independent objects placed “into” space. Instead, particles are localized, self-maintaining coherence-patterns. Their discrete particle-like features emerge because their internal coherence structure is tightly bounded and continuously preserved by the local update rules of the network.

### 2.2 Minimal Local Rules and Assumptions
*TODO: List the minimal rule set governing local updates (causality, adjacency, budget accounting, update resolution order). State assumptions and scope.*

### 2.2 Interpretive Rules
**The Principle of Node Inertia:**  
The node network never strains, never moves, and never resists. All energy belongs exclusively to the pattern. All difficulty in motion arises from the pattern’s requirement to maintain internal coherence under the fixed update rule. If a demanded configuration cannot be self-consistently re-instantiated across adjacent nodes, the pattern destabilizes and collapses into simpler, incoherent excitations.


### 2.3 The Node State Bundle
**Cadence‑based Strain (CaBS)**  
CaBS is the mechanism by which node cadence and adjacency determine coherence capacity. Define CaBS once, then use the component symbols **B** (Budget), **S** (Strain), and **τ** (effective cadence) in all equations, simulations, and logs. CaBS is referenced in prose when describing the mechanism; the symbols are used in math.

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

### 2.6 The Incoherent Channel (H): Pattern-Dependent Yield and Collapse
*Hypothesis: Coherence is a finite resource. A node network undergoes a yield event when the update demand relative to local capacity, scaled by the pattern's intrinsic stability, exceeds a critical threshold.*

**Pattern Stability Factor ($\Gamma_p$):**
We introduce a dimensionless pattern stability factor $\Gamma_p$ that quantifies a pattern's ability to maintain directional coherence under applied update demand. $\Gamma_p$ encodes adjacency reinforcement and cadence coupling—how well the pattern's topology and update timing preserve phase alignment. 
*   $\Gamma_p > 1$: Robust patterns (e.g., tightly bound loops, high-density lattices).
*   $\Gamma_p < 1$: Fragile patterns (e.g., loosely bound waves).

**The Yield Criterion (Static Form):**
A node collapses into the incoherent energy channel (H) when the pattern-specific update demand ($S_p$) relative to the local budget ($B$) exceeds the network's yield constant ($\kappa_{\text{yield}}$) scaled by the pattern's stability:
$$\frac{S_p}{B} \ge \kappa_{\text{yield}} \Gamma_p$$

**H-Density and Entropy:**
Incoherent energy is modeled as a local density field $\rho_H$. Thermodynamic entropy ($S_{\text{cg}}$) emerges as the coarse-grained statistical summary of this accumulated "accounting debris":
$$\rho_H(x,t) \equiv \frac{\Delta E_{\text{incoh}}(x,t)}{\Delta V}$$
$$S_{\text{cg}} \sim \int \rho_H \ln \rho_H \, dV$$

**Cross references:** See Sec. 4.4 The Node Ledger for the local partition identity; Sec. 4.5 Boundary Ledger and Tests for interface experiments; Sec. 11 Computational Implementation Layer for logging and simulation protocols; Sec. 13 Predictions and Falsifiable Tests for experimental calibration plans.

### 2.7 Incoherent Channel (H) — Definition and Manifestations
### 2.71 Coherence-Strain and Coherence-Shedding
When a pattern moves through regions of high utilization, its degradation proceeds through two stages:

* **Coherence-Strain ($S$):** The accumulation of coherent update demand on the local node network. As the incoming load ($S$) increases relative to the available budget ($B$), the local resolution latency increases.
* **Coherence-Shedding ($\Delta H$):** When the local processing capacity is exceeded, the pattern undergoes a shedding event. Unresolvable exactions are rejected and fall out of the coherent ledger, collapsing into incoherent excitations ($\Delta H$), observed macroscopically as heat.

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

### 2.8 Topology of the Node Network
Because the update rules rely solely on fixed local adjacency, the global topology of the node network remains unconstrained. Permissible configurations include:

* A torus or hypertorus  
* A finite bubble  
* A compact manifold  
* A multiply connected space  
* A closed but boundaryless topology  

Any global structure is valid, provided it preserves fixed local adjacency and a uniform update rule across all nodes.


---

## 3. Capacity Limits and Divergence‑Free Behavior
### 3.0 Update Mechanics
To clarify the mechanics of the spatial-temporal step, we distinguish two complementary perspectives of a single network event:

* **Re-instantiation:** The temporal update of the pattern. Each tick, the node network recalculates and re-instantiates the pattern according to its fixed local transition rules.
* **Re-embedding:** The spatial placement of the pattern. This describes how the updated coherence-structure is placed back into the physical node layout.

Re-instantiation and re-embedding occur simultaneously; they represent the temporal and spatial dimensions of the same update step.


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

### 3.4 Critical Threshold and Phase Transition
The "Redline" of the vacuum is defined by the approach to $B \to 0$. As the budget is exhausted, the pattern-dependent yield criterion is triggered:
$$\frac{S_p}{B} \ge \kappa_{\text{yield}} \Gamma_p$$

Dynamic loading (CaBS) lowers the effective threshold, making rapid increases in update demand more likely to trigger a collapse into H. In this regime, the node ensemble can no longer sustain the coherent update demand of the primary pattern. To prevent a geometric singularity, the node network undergoes a **Phase Transition**, reconfiguring local node states into new, simpler patterns (e.g., Pair Production). This mechanism replaces the mathematical "shambles" of the GR singularity with a physically finite, high-strain core.

### 3.5 The Netzero Energy Principle
SVET adopts a **Netzero** energy interpretation rather than the quantum field theory concept of zero-point energy. The node network itself possesses zero net energy in its idle state. All physical energy is an accounting of active, coherent patterns moving through the network.

To maintain operations without divergence, we define a non-zero **Floor Budget ($B_0$)**—the baseline coherent-processing capacity of idle nodes. This is a structural threshold of the network, not stored energy, vacuum energy, or dark energy.

---

## 4. Flux Algebra

### 4.1 Flux as Directional Coherent Update Demand
*TODO: Provide the SVET definition of flux: the directional component of coherent exaction attempting to propagate across adjacency. Clarify notation and units.*

### 4.2 Flux Addition and Cancellation
*TODO: Formalize vector addition rules for flux, including cancellation, superposition, and normalization constraints.*

### 4.3 Propagation, Reflection, and Refraction
*TODO: State local update rules that produce propagation, reflection, and refraction. Include boundary interaction rules and examples.*

### 4.4 The Node Ledger (Conservation of Energy)

**Statement (operational):** Conservation of energy in SVET is a bookkeeping identity of the node‑network update. Local update demand is partitioned at each node according to the success or failure of the pattern‑dependent yield criterion and the local CaBS dynamics.

**Partition identity (node level):**


\[
I_{\text{in}} = I_{\text{refl}} + I_{\text{trans}} + \Delta H
\]


Equivalently, in normalized form:


\[
R + T + H = 100\%
\]



**Component definitions and locality**
- **\(I_{\text{refl}}\) (Coherent Rejection / Reflection):** a *surface* event. Occurs when a neighbor node (or interface) cannot accept the incoming coherent demand; the rejected portion remains coherent and carries phase information away from the boundary.  
- **\(I_{\text{trans}}\) (Coherent Propagation / Transmission):** the coherent portion successfully accepted by the neighbor and available for further coherent propagation.  
- **\(\Delta H\) (Incoherent Energy / H):** a *bulk* event. Energy diverted into the incoherent channel when the pattern‑dependent yield criterion is met (coherence → incoherence). \(\Delta H\) is the local increment of incoherent energy that may later manifest as heat, photochemistry, fluorescence, photoemission, mechanical damage, etc.

**Link to yield and CaBS dynamics**  
The partition depends on the local budget \(B\), pattern demand \(S_p\), pattern stability \(\Gamma_p\), and dynamic loading (CaBS) factors. In compact form:


\[
\text{Yield if}\quad \frac{S_p}{B}\,\Gamma_p\,\Phi(\dot S_p,\tau_{\text{eff}}) \ge \kappa_{\text{yield}},
\]


where \(\Phi(\dot S_p,\tau_{\text{eff}})\) encodes rate/cadence dependence. If the yield condition is met at the node, the accepted coherent propagation fails and the corresponding energy is diverted into \(\Delta H\); otherwise the ledger partitions into reflection and transmission according to local acceptance rules.

**Practical notes**
- **Surface vs bulk:** Always preserve the distinction in derivations and experiments: reflection is a boundary accounting event; H production is a bulk, post‑acceptance event.  
- **Conservation semantics:** This identity is bookkeeping — energy is redistributed between coherent and incoherent channels; no external creation or destruction is invoked.  
- **Cross references:** See Sec. 2.6 (Incoherent Channel and Yield), Sec. 4.5 (Boundary Ledger and Tests), Sec. 11 (Computational Implementation) for logging and simulation protocols, and Sec. 13 (Predictions) for experimental tests.

*TODO:* Derive the partition identity from the node update algorithm and show how global conservation follows from local ledger reconciliation.


### 4.5 Boundary Ledger and Tests
**Note:** Boundary partitioning depends on the pattern‑dependent yield criterion defined in Sec. 2.6 Incoherent Channel (H). See Sec. 4.4 The Node Ledger for the node‑level partition identity and Sec. 11 Computational Implementation Layer for the simulation logging checklist used to validate boundary predictions.

**Summary**  
In SVET, boundary interactions are governed by local CaBS accounting. Incident coherent flux is partitioned at the surface into coherent reflection, coherent transmission, and incoherent bulk loss. Reflection is a surface accounting shock (coherent rejection), not a primary decoherence event. Decoherence (H) occurs only after coherent flux is accepted into the medium and then loses directional coherence.

**Boundary Ledger Identity**  
The local energy ledger at a boundary node satisfies:


\[
I_{\text{in}} = I_{\text{refl}} + I_{\text{trans}} + I_{\text{heat}}
\]


where:
- \(I_{\text{refl}}\) is **coherent reflection** (surface event),  
- \(I_{\text{trans}}\) is **coherent transmission** (accepted flux),  
- \(I_{\text{heat}}\) is **incoherent bulk loss** (H channel).

**Local Acceptance Rule**  
For a boundary node with Budget \(B\) and local Strain \(S\), the instantaneous transmission fraction may be expressed as:


\[
T \equiv \frac{I_{\text{trans}}}{I_{\text{in}}} \approx \frac{B}{B + S}
\]


and the effective cadence (delay per update) is:


\[
\tau_{\text{eff}} = \tau_0\left(1 + \left(\frac{S}{B}\right)^\beta\right)
\]


These relations fix reflection and absorption once \(B\) and \(S\) are specified for the interface and bulk.

**Experimental Slab Test Specification (Normal Incidence)**

1. **Setup**  
   - Monochromatic source with known incident intensity \(I_{\text{in}}\).  
   - Thin slab of material with well‑characterized surface and bulk CaBS parameters \(B_{\text{surf}}, S_{\text{surf}}, B_{\text{bulk}}, S_{\text{bulk}}\).  
   - Instruments: calibrated photodetectors for reflected and transmitted coherent intensity; calorimeter or bolometer for bulk heating \(H\).

2. **Measurements**  
   - Measure \(R = I_{\text{refl}}\), \(T = I_{\text{trans}}\), and \(H\) (energy deposited as incoherent channel).  
   - Verify ledger identity \(R + T + H \approx I_{\text{in}}\) within experimental error.

3. **Predictions to test**  
   - Vary surface \(B_{\text{surf}}\) (e.g., by coating) and observe predicted change in \(R\) with \(T\) and \(H\) constrained by CaBS accounting.  
   - Under intense pumping, measure change in \(S\) and resulting shifts in \(T\) and \(\tau_{\text{eff}}\) (pump‑induced refractive index shifts).

4. **Controls**  
   - Use nonabsorbing reference (e.g., fused silica) to validate coherent reflection baseline.  
   - Use pump‑probe to separate instantaneous coherent rejection from slower incoherent absorption dynamics.

**Simulation Logging Checklist**  
Record per node and per timestep:
- **Coherent flux vector** (magnitude and orientation)  
- **Local B, S, τ_eff**  
- **I_refl, I_trans, ΔH** (energy moved into incoherent channel)  
- **Phase coherence metric** (e.g., vector alignment index)  
- **Boundary ledger reconciliation events** (rejection vs acceptance)

**Cross‑references**  
- Cross‑reference this subsection in **Section 5 (Emergent Wave Mechanics)** for interference consequences.  
- Cross‑reference in **Section 10 (Material Response & Dispersion)** for mapping H to material observables.  
- Cross‑reference in **Section 12 (Predictions)** for experimental claims.  
- Refer to **Section 11 (Computational Implementation)** for logging and simulation details.


---

## 5. Emergent Wave Mechanics
See Section 4.5 (Boundary Ledger and Tests) for the local ledger that determines surface reflection vs transmission.

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
### 8.1 Relativistic Latency and Stability Limits
Relativistic effects emerge from local processing constraints. When a pattern experiences high strain ($S$) relative to the available budget ($B$), the network requires additional ticks to resolve the pattern’s adjacency constraints.

* **Time Dilation ($\Delta \tau$):** Resolution latency increases as the effective cadence ($\tau_{\text{eff}}$) slows in high-strain regions.
* **Stability under Strain ($\Gamma_p$):** If the strain-to-budget ratio exceeds the pattern’s stability threshold ($\Gamma_p$), the pattern reaches its limit and fractures.
* **Tidal Gradient Response:** In regions with steep spatial gradients of cadence ($\nabla \tau_{\text{eff}}$) or extreme $S/B$ variation, different parts of an extended pattern experience uneven latency. This destabilizes the internal structure, stretching it until localized $\Gamma_p$ collapse occurs.
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
Map H (incoherent flux) from Section 4.5 to material sinks (phonons, fluorescence, photoemission)

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
Log fields listed in Section 4.5 Simulation Logging Checklist for reproducible runs.

### 12.4 Numerical Stability and Convergence
**Simulation cross‑references:** Implement the logging fields required to validate Sec. 2.6 (pattern stability Γ_p and yield events) and Sec. 4.5 (boundary ledger tests). See Sec. 2.6 Incoherent Channel (H) for definitions of S_p, B, Γ_p and Sec. 13 Predictions and Falsifiable Tests for the calibration experiments to reproduce in simulation.

*TODO: Provide notes on timestep selection, stability criteria, and convergence tests.*



---

## 13. Predictions and Falsifiable Tests
Possible 13.6 Reflectivity, Decoherence, Plastic deformation. Experimental slab test described in Section 4.5 provides a direct falsifiable test of SVET partitioning.
**Experimental dependencies:** The predictions below assume the pattern‑dependent yield formalism of Sec. 2.6 Incoherent Channel (H) and the node partition identity of Sec. 4.4 The Node Ledger. Simulation protocols in Sec. 11 Computational Implementation Layer provide the reproducible logging required to compare measured R, T, and H against SVET predictions.

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

### 12.6 The Yield Ramp Test
*Simulation:* Locally increase update demand ($S_p$) at a node ensemble and measure the critical $S/B$ ratio where coherent amplitude collapses into the H-channel.
*Target:* This test uses a reference pattern with $\Gamma_p = 1$ under slow loading to isolate the universal constant $\kappa_{\text{yield}}$.

### 12.7 Loop Integrity and Confinement
*Simulation:* Model a coherent loop (particle) under increasing external strain. 
*Target:* Verify if a loop yield event produces energy-conserving pair excitations. For high $\Gamma_p$ patterns, yield events are irreversible, providing a node-network explanation for quark confinement.

### 12.8 Measurement Statistics (Born Rule Emergence)
*Simulation:* Model a detector as a localized strain source. 
*Target:* Demonstrate that "Wavefunction Collapse" statistics emerge from the yield event of the wave pattern, converging to Born-rule frequencies over repeated trials.

### 12.9 Coherence Recovery Test
*Simulation:* After a near-yield ramp, reduce $S_p$ and observe whether the pattern re-establishes coherence. 
*Target:* Robust patterns (high $\Gamma_p$) should recover; fragile patterns may not. Record hysteresis and recovery times to distinguish reversible vs. irreversible yield.

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
