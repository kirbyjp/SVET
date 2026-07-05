---
title: "Static Vacuum Exaction Theory (SVET)"
subtitle: "A capacity-limited Planck-scale physical vacuum as a unified foundation for General Relativity and Quantum Gravity"
author: 
  - John Kirby
date: "June 2026"
abstract: |
  This document presents Static Vacuum Exaction Theory (SVET), a discrete resource-accounting model of the physical vacuum. SVET models the vacuum as a network of Planck-scale nodes with finite update budgets and local update rules. From these primitives we derive emergent wave mechanics, a divergence-free account of quantum excitations, finite-core black holes, and a cadence-based mapping to gravitational phenomena. The framework is written as a living Markdown document (MathJax/LaTeX compatible) intended for iterative development, Pandoc conversion, and eventual arXiv/journal submission.
keywords: [Quantum Gravity, General Relativity, Substrate Physics, Discrete Vacuum, Singularities, CaBS]
geometry: margin=1in
fontsize: 11pt
header-includes:
  - \usepackage{amsmath}
---

# Static Vacuum Exaction Theory (SVET)  
### A capacity‑limited Planck‑scale physical vacuum as a unified foundation for GR and QG

---

2. Ontology of the Vacuum
3. Capacity Limits and Divergence‑Free Behavior
4. Flux Algebra
5. Emergent Wave Mechanics
6. Hilbert‑Space Correspondence
7. QFT Correspondence Layer
8. GR Correspondence Layer
9. Causal Boundaries
10. Measurement and Decoherence
11. Material Response & Dispersion
12. Computational Implementation Layer
13. Predictions and Falsifiable Tests
14. Emergent Continuum
15. Correspondence With Observables
16. Open Questions and Future Work

---

## 0. Notes on this document
*This file is the living source for SVET. It is Markdown + MathJax (LaTeX math) and is intended to be converted to LaTeX/PDF via Pandoc for arXiv or journal submission. Use the Git history for versioning; keep the filename `theory.md` as the single source of truth.*

---

## 1. Introduction

### Preface: Etymological Context
The acronym SVET (Static Vacuum Exaction Theory) also mirrors the word for "world" and "light" in several European languages. This dual meaning reflects the model’s purpose: to describe the fundamental structure of the cosmos (the world) and the propagation of coherent excitations (light) through a unified, capacity-limited node set.

### 1.1 What the Node Space Is
The node space is the vacuum—the same physical vacuum studied in quantum field theory, cosmology, and high‑energy physics. SVET does not introduce an additional medium; it reinterprets the existing vacuum as a static set of update sites whose localized, discrete excitations manifest as physical patterns.

The node space supports waves rather than point‑like particles. What experimental physics registers as “particles” are localized, self‑maintaining coherence‑patterns whose tightly confined structure produces particle-like behavior.

*TODO: Describe the motivation for SVET — resolving GR singularities and QFT divergences through a finite, capacity‑limited node space. Provide a concise roadmap of the paper and summarize the main claims and predictions.*

### 1.2 Epistemological Foundations: SVET vs. Quantum Field Theory

To establish the foundational boundaries of this framework, we must clarify the epistemological distinction between continuous wave-particle formulations and discrete exaction bookkeeping:

> Quantum Field Theory (QFT) predicts what you will observe but does not describe what is happening; SVET describes what is happening and therefore explains why you observe it.

Continuous field theory relies on abstract operator mathematics, complex probability amplitudes, and non-local wave-packet evolutions. While these mathematical tools yield highly accurate macroscopic predictions, they treat the background coordinate space as a continuous, passive stage, leaving the underlying physical mechanism of state transitions unmapped.

SVET grounds physical events in the behavior of a discrete, capacity‑limited vacuum. Instead of relying on continuous fields or abstract amplitudes, it describes physical phenomena through the local interactions of a fixed set of update sites. This approach provides a direct, mechanism‑level account of how observable events arise, offering a descriptive framework that complements the predictive strengths of quantum field theory.

---

## 2. Ontology of the Vacuum

### 2.0 Ontology of the Vacuum Overview
This chapter details the fundamental ontology of the physical vacuum within the SVET framework. We establish the node network as the primary, static, non-coordinate system of discrete update sites, from which space, time, and coherent matter emerge. By analyzing localized coherence configurations and their local rules, we formalize the boundary between coherent propagation and incoherent dissipation, defining the structural limits of physical patterns.

### 2.1 The Planck‑Scale Physical Vacuum

The SVET vacuum is a static, Lorentz-invariant node network whose local states fluctuate near their minima without bulk motion or a preferred reference frame. Lorentz symmetry emerges naturally from the isotropic symmetry of the local node update rules; macroscopic physical excitations are coherent wave patterns propagated by the node network rather than independent, self-contained ontological objects. The invariant causal speed limit $c$ arises from the absolute, structural one-adjacency-hop-per-tick propagation limit of the network.

#### 2.1.1 Quantitative Scale Structure of the Vacuum

*TODO: Provide quantitative scale comparisons to illustrate why the node network must support coherence across many orders of magnitude. Include the following reference values:*

- *Electron cloud radius (1s orbital): ~0.05–0.1 nm ($50,000\text{--}100,000\text{ fm}$)*  
- *Nucleus radius: ~1–5 fm ($100,000\times$ smaller than the electron cloud)*  
- *Proton radius: ~0.84 fm*  
- *Quark confinement region: ~0.3 fm*  
- *Planck length: ~$10^{-20}\text{ fm}$*

*These scales imply that a single node must support coherent behavior across at least five orders of magnitude, and potentially up to nineteen orders of magnitude when comparing quark-scale structure to the Planck length.*

*TODO: Note the theoretical upper bound on update frequency: the Planck frequency, defined as*  

$$f_{\text{Planck}} = \frac{1}{t_{\text{Planck}}} \approx 10^{43}\text{ Hz}$$

*This establishes the maximum conceivable cadence for any physical update process and constrains the upper bound of node network timing behavior.*

### 2.1.2 Patterns as Particles

Within the node network, physical entities are not independent objects placed “into” space. Instead, particles are localized, self-maintaining coherence-patterns. Their discrete particle-like features emerge because their internal coherence structure is tightly bounded and continuously preserved by the local update rules of the network.

*TODO: Provide relative scale scaling factors to contextualize coherence confinement. Address the spatial volume ratios of these distinct physical domains, emphasizing that the spatial profile of the electron orbital spans five orders of magnitude relative to the proton core, while the nuclear confinement radius restricts multi-nucleon configurations to a narrow spatial volume relative to the outer electron cloud boundary. These scaling ratios will be mapped to formal coherence-geometry descriptions in later sections.*

### 2.2 Minimal Local Rules and Assumptions

The node set operates under a minimal set of local rules that govern all coherent and incoherent update behavior. These rules define the structural constraints from which space, time, and physical propagation emerge.

**1. Locality and Adjacency**  
Each node interacts only with its immediate neighbors. All propagation, strain exchange, and ledger reconciliation occur across adjacency links; no long-range or nonlocal updates are permitted.

**2. Causality and Update Ordering**  
Updates occur in a fixed, globally consistent tick order. A node may only incorporate information from the previous tick of its neighbors, ensuring strict causal structure and preventing retroactive modification of prior states.

**3. Budget Accounting**  
Each node maintains a finite update budget that constrains how much coherent routing it can support per tick. Competing demands for propagation are resolved by comparing local strain, bias, and available budget.

**4. Resolution of Competing Flux**  
When multiple coherent demands attempt to traverse the same adjacency, the node resolves them according to least-cost routing preferences derived from local strain and bias. Excess demand is diverted into the incoherent channel.

**5. No Node Motion or Deformation**  
Nodes do not move, stretch, or rearrange. All geometric behavior arises from routing preferences and cadence variations, not from changes in the underlying node-set structure.

These minimal rules define the operational node-set foundation from which coherent patterns, propagation geometry, and causal structure emerge.
#### 2.2.1 Interpretive Rules
**The Principle of Node Inertia:**  
The node network never strains, never moves, and never resists. All energy belongs exclusively to the pattern. All difficulty in motion arises from the pattern’s requirement to maintain internal coherence under the fixed update rule. If a demanded configuration cannot be self-consistently re-instantiated across adjacent nodes, the pattern destabilizes and collapses into simpler, incoherent excitations.

#### 2.2.2 Update Mechanics
To clarify the mechanics of the spatial-temporal step, we distinguish two complementary perspectives of a single network event:
* **Re-instantiation:** The temporal update of the pattern. Each tick, the node network recalculates and re-instantiates the pattern according to its fixed local transition rules.
* **Re-embedding:** The spatial placement of the pattern. This describes how the updated coherence-structure is placed back into the physical node layout.

Re-instantiation and re-embedding occur simultaneously; they represent the temporal and spatial dimensions of the same update step.

### 2.3 The Node State Bundle
**Cadence‑based Strain (CaBS)**  
CaBS is the mechanism by which node cadence and adjacency determine coherence capacity. Define CaBS once, then use the component symbols **B** (Budget), **S** (Strain), and **τ** (effective cadence) in all equations, simulations, and logs. CaBS is referenced in prose when describing the mechanism; the symbols are used in math.

- **B** — capacity (node budget)  
- **S** — strain (current load)  
- **B₀** — baseline capacity (resting budget)  
- **τ₀** — base tick (node network fundamental tick)  
- **τ_eff** — effective cadence (local update delay)  
*TODO: Define units, ranges, and physical interpretation for each variable. Provide canonical initial conditions and normalization conventions.*

### 2.4 Directional Phase Encoding

In SVET, phase is not represented through complex amplitudes but through the orientation and timing of coherent update demand. A pattern’s local phase is encoded in the directional alignment of its flux vectors and the cadence delays accumulated during propagation.

**Directional Encoding of Phase**  
The orientation of coherent flux across adjacency links determines the instantaneous phase of a propagating pattern. Two patterns with identical amplitudes but differing flux orientations represent distinct phase states.

**Cadence Delay as Phase Shift**  
Local variations in effective cadence $\tau_{\text{eff}}$ introduce timing offsets that act as phase shifts. A delay of one tick corresponds to a discrete phase increment, and accumulated delays reproduce continuous phase evolution in the long-wavelength limit.

This directional-timing encoding reproduces the interference behavior associated with complex phase factors while remaining fully grounded in local, real-valued update rules.

### 2.5 Dual‑Channel Propagation

Propagation across the node set occurs through two distinct channels: a coherent channel that preserves pattern structure and an incoherent channel that records excess update demand as heat.

**1. Coherent Channel (Pattern-Preserving)**  
The coherent channel carries directional flux that maintains the internal structure of a pattern. As long as local budget constraints are satisfied, coherent flux propagates according to least-cost routing preferences determined by strain and bias.

**2. Incoherent Channel (Heat / Ledger Channel)**  
When coherent update demand exceeds the available local budget, the excess is diverted into the incoherent channel. This channel records non-directional update activity that cannot contribute to pattern maintenance. It represents the local dissipation of coherence.

**3. Decoherence as Budget Overflow**  
A pattern decoheres when a sufficient fraction of its update demand is forced into the incoherent channel. This process is irreversible: once directional coherence is lost, the pattern cannot reconstruct its original structure from heat-channel activity.

The dual-channel structure provides a natural mechanism for decoherence, dissipation, and the emergence of classical behavior from coherent propagation.

### 2.6 The Incoherent Channel (H): Definitions, Yield, and Manifestations

#### 2.6.1 Core Definitions and the Yield Criterion
Coherence is a finite resource. A node network undergoes a yield event when the update demand relative to local capacity, scaled by the pattern's intrinsic stability, exceeds a critical threshold.

**Pattern Stability Factor ($\Gamma_p$):**
We introduce a dimensionless pattern stability factor $\Gamma_p$ that quantifies a pattern's ability to maintain directional coherence under applied update demand. $\Gamma_p$ encodes adjacency reinforcement and cadence coupling—how well the pattern's topology and update timing preserve phase alignment. 
*   $\Gamma_p > 1$: Robust patterns (e.g., tightly bound loops, high-density lattices).
*   $\Gamma_p < 1$: Fragile patterns (e.g., loosely bound waves).

**The Yield Criterion (Static Form):**
A node collapses into the incoherent energy channel (H) when the pattern-specific update demand ($S_p$) relative to the local budget ($B$) exceeds the network's yield constant ($\kappa_{\text{yield}}$) scaled by the pattern's stability:
$$\frac{S_p}{B} \ge \kappa_{\text{yield}} \Gamma_p$$

### 2.6.2 Coherence‑Strain and Coherence‑Shedding

When a pattern moves through regions of high utilization, its degradation proceeds through two discrete stages:

**• Coherence‑Strain ($S$):**  
The accumulation of coherent update demand on the local node set. As the incoming load $S$ increases relative to the available budget $B$, the local resolution latency rises and the pattern accumulates internal strain energy. This strain energy reflects the mismatch between the pattern’s preferred propagation geometry and the cadence‑limited routing permitted by the surrounding node set.

**• Coherence‑Shedding ($\Delta H$):**  
When the local processing capacity is exceeded, the pattern undergoes a shedding event. Unresolvable update demand is rejected and diverted out of the coherent ledger, collapsing into incoherent excitations $\Delta H$, observed macroscopically as heat.

As internal strain energy accumulates, the pattern’s coherence integrity progressively weakens. The rising tension between its internal wave‑geometry and the cadence‑limited routing environment eventually triggers coherence‑shedding, leading to partial or complete collapse into the incoherent channel (H).

#### 2.6.3 Physical Nature and Manifestations of H
In SVET, **H** denotes *incoherent energy* — energy that has left the coherent propagation channel and no longer carries directional phase information. Heat is one possible macroscopic manifestation of H, but H is a node network-level category that can produce multiple physical outcomes depending on the local material and boundary physics.

Formally, a coherence $\to$ incoherence transition occurs when the local load and cadence demand exceed adjacency’s capacity to maintain phase alignment:
$$\text{If}\quad \text{Strain} \; \lor \; \text{CaBS demand} \;>\; \text{Adjacency coherence capacity} \quad\Rightarrow\quad \text{Coherent}\;\to\;\text{Incoherent (H)}$$

Macroscopic manifestations of H include:
*   **Thermal phonons (heating)** — incoherent energy couples to lattice vibrations.  
*   **Photochemistry / UV curing** — incoherent energy drives chemical bond rearrangements.  
*   **Fluorescence / radiative decay** — incoherent excitations re‑emit photons at shifted energies.  
*   **Photoelectric emission** — incoherent energy ejects electrons from material.  
*   **Structural failure (plastic deformation, fracture)** — coherent stress patterns collapse into incoherent modes that manifest as mechanical damage.  
*   **Other sinks** — any process that accepts incoherent energy (e.g., metastable trapping, nonradiative decay).

#### 2.6.4 Analytical Advantages & Experimental Integration
*   **Unified mechanism:** Optical decoherence, heating, chemical reactions, and mechanical failure are all instances of the same node network event: loss of coherence.  
*   **Predictive accounting:** The CaBS ledger predicts how much energy remains coherent vs. how much becomes H; the material properties determine the final sink.  
*   **Falsifiable signatures:** The partitioning ratio (coherent : incoherent) at interfaces and under pump conditions yields measurable predictions (e.g., reflected fraction, fluorescence yield, temperature rise).
*   **Simulation Tracking:** Track coherent flux and H accumulation separately in simulations. Report H as an energy flux into the incoherent channel, then map H to specific observables using material response models (phonon coupling constants, reaction cross sections, etc.).

**H-Density and Entropy:**
Incoherent energy is modeled as a local density field $\rho_H$. Thermodynamic entropy ($S_{\text{cg}}$) emerges as the coarse-grained statistical summary of this accumulated "accounting debris":
$$\rho_H(x,t) \equiv \frac{\Delta E_{\text{incoh}}(x,t)}{\Delta V}$$
$$S_{\text{cg}} \sim \int \rho_H \ln \rho_H \, dV$$

**Cross references:** See Sec. 4.4 The Node Ledger for the local partition identity; Sec. 4.5 Boundary Ledger and Tests for interface experiments; Sec. 11 Computational Implementation Layer for logging and simulation protocols; Sec. 13 Predictions and Falsifiable Tests for experimental calibration plans.

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

### 3.1 Finite Excitation Capacity

Each node in the SVET node set supports a finite excitation capacity, expressed by the dimensionless excitation norm (as defined in Section 3.7, Axiom 1):
$$0 \le \eta(x) \le 1$$

The upper bound $\eta = 1$ represents the microphysical saturation ceiling, corresponding to the maximum coherent update demand that a node can process within a single tick. This ceiling is enforced by the Margolus–Levitin bound on state-change rates (Section 3.7, Axiom 2) and ensures that no node can host arbitrarily large field amplitudes or arbitrarily high-frequency excitations.

Because excitation is bounded, all local physical quantities derived from excitation—such as strain $S_{ij}$, bias $B_a$, and coherence cost $C(x,v)$—inherit finite upper limits. These bounds prevent ultraviolet divergences and ensure that all local update behavior remains well-defined.

### 3.2 Finite Update Cadence (τ_eff)

The effective cadence $\tau_{\text{eff}}$ of a pattern reflects the local difficulty of resolving its coherent update demand. As strain increases relative to the available budget, the local resolution latency grows. A minimal phenomenological form capturing this slowdown is:

$$\tau_{\text{eff}} = \tau_0 \left(1 + \left(\frac{S}{B}\right)^\beta\right)$$

where:
- $\tau_0$ is the baseline cadence in the low-strain limit,
- $S$ is the local coherent strain,
- $B$ is the available update budget,
- $\beta$ is a dimensionless exponent controlling how sharply cadence increases under load.

Larger values of $\beta$ correspond to more abrupt cadence penalties, while smaller values produce smoother slowdowns. Regardless of the specific form, all admissible cadence functions must satisfy:
- $\tau_{\text{eff}} \to \tau_0$ as $S/B \to 0$,
- $\tau_{\text{eff}} \to \infty$ as $S/B \to \infty$.

As established in the Section 3.7 Axiom 5 ontology, this cadence collapse is strictly a pattern-level phenomenon. The underlying nodes in the node set continue to update at the invariant propagation speed $c$ (one adjacency hop per tick); what collapses under load is the ability of extended coherent structures to exploit that raw capacity. This ensures that cadence slowdown remains finite under normal conditions and diverges asymptotically only when the pattern's coherent update demand fully saturates the local node capacity.

### 3.3 Why Divergences Cannot Occur

SVET forbids ultraviolet divergences because all local update behavior is governed by finite, capacity-limited quantities. Three structural constraints enforce this:

1. **Finite Excitation:**  
   The excitation norm satisfies $0 \le \eta \le 1$, preventing unbounded field amplitudes.

2. **Finite Update Capacity:**  
   Each node’s update rate is bounded by the Margolus–Levitin limit:
   $$u(\eta) \le u_{\text{node,max}}$$

3. **Finite Cadence Response:**  
   The effective cadence $\tau_{\text{eff}}$ diverges only when coherent demand exceeds the available budget, ensuring that no physical process can demand infinite update throughput.

Because all local quantities—excitation, strain, bias, cadence, and ledger updates—are bounded, no SVET process can produce the infinities that plague continuum field theories. Divergences are replaced by well-defined capacity ceilings and pattern-level cadence collapse.

### 3.4 Critical Threshold and Phase Transition
The "Redline" of the vacuum is defined by the approach to $B \to 0$. As the budget is exhausted, the pattern-dependent yield criterion is triggered:
$$\frac{S_p}{B} \ge \kappa_{\text{yield}} \Gamma_p$$

Dynamic loading (CaBS) lowers the effective threshold, making rapid increases in update demand more likely to trigger a collapse into H. In this regime, the node ensemble can no longer sustain the coherent update demand of the primary pattern. To prevent a geometric singularity, the node network undergoes a **Phase Transition**, reconfiguring local node states into new, simpler patterns (e.g., Pair Production). This mechanism replaces the mathematical singularity of General Relativity with a physically finite, high-strain core.

### 3.5 The Netzero Energy Principle

SVET adopts a **Netzero** energy interpretation rather than the traditional quantum field theory concept of zero-point energy. The node set itself possesses zero net energy in its static configuration. All physical energy is a ledger accounting of active, coherent pattern exactions compelling the node set to spend its available local update budgets.

#### The Static Vacuum and Budget Availability
The node set does not perform background updates in empty space. The tick budget is a finite capacity that remains available until pattern exactions require expenditure. In empty space, nodes do not perform updates other than to maintain their node bias [1]. Updates occur only when active patterns demand instantiation.

No exaction means no expenditure of budget.

#### The Local Floor Budget ($B_0(x)$)
The Floor Budget is a localized structural quantity defining the minimum available tick-budget a node must expend to exist as a structural element of adjacency:
$$B_0(x) > 0$$
Because distant pattern exactions propagate across adjacency, the cumulative background exaction density varies across the cosmos. Thus, $B_0(x)$ is minimal in deep voids, higher in regions of moderate mass density, and reaches extreme values near gravatar boundaries. 

The Local Floor Budget $B_0(x)$ is not an independent vacuum reservoir or background energy field; it is the local structural floor induced entirely by the collective pattern exactions of the universe.

Because the node set does not possess or store energy independently, the conservation of energy is the exact conservation of local coherence constraints [1]. When patterns interact, their combined coherence structures must reconcile their update demands across the adjacent node set into a new, self-consistent configuration. No physical energy is transferred; instead, the underlying exaction-driven coherence constraints are redistributed according to what we may think of as the local ledger conservation identity [1]:
$$I_{\text{in}} = I_{\text{refl}} + I_{\text{trans}} + \Delta H = 100\%$$
Thus, energy conservation is not an arbitrary physical law imposed on the universe, but the exact mathematical consequence of preserving pattern identity across discrete temporal ticks.

#### 3.5.1 The Vacuum Catastrophe and Horizon Capacity Constraint
With the Netzero principle, the static vacuum, and the ledger identity established, we can now formalize the global capacity constraint of the node set that resolves the long‑standing vacuum discrepancy. In continuous quantum field theory, the absolute sum of all zero-point modes yields an unphysical vacuum energy density that exceeds the observed cosmological constant by roughly 120 orders of magnitude (the $10^{122}$ "vacuum catastrophe"). SVET predicts that this pathology is a category error: QFT has mistakenly interpreted the node set's maximum update capacity as an active, gravitating exaction load.

To formalize this constraint, let:
*   $\epsilon_{\text{cap}}$ be the maximum possible update capacity per node (per tick, per node).
*   $\epsilon_0(x)$ be the baseline structural exaction cost a node expends to exist as an element of adjacency.
*   $C = \frac{\epsilon_{\text{cap}}}{\epsilon_0(x)}$ be the capacity-to-load ratio of an individual node.
*   $N_H$ be the total number of discrete nodes contained within a single cosmic horizon volume.

The vacuum catastrophe is resolved as a finite, non-singular capacity constraint of the node set:
$$C\,N_H \approx 10^{122} \qquad \text{or} \qquad \frac{\epsilon_{\text{cap}}}{\epsilon_0(x)}\,N_H \approx 10^{122}$$

This constraint states that the total available, unused update capacity of all nodes inside a cosmic horizon volume exceeds the local structural exaction cost actually in use by approximately $10^{122}$. In words: a historically severe discrepancy between theoretical prediction and observation is recognized as a structural, scale-bridging constant of the node set, indicating that the baseline vacuum of empty space operates in a highly under-utilized state [1].

### 3.6 CaBS Primitive Rules (Cadence–Budget–Strain)

The Cadence-Budget-Strain (CaBS) framework defines the node network's localized update engine. It formalizes how local strain, available processing budget, and temporal dilation interact to govern pattern propagation.

#### Core Definitions
*   **Strain ($S$):** The localized update load on the node network, representing the density of coherence demands that must be resolved per tick.  
*   **Budget ($B$):** The remaining coherent processing headroom of a node, representing the fraction of update capacity not yet consumed by localized strain.  
*   **Dilation ($\alpha$):** The dimensionless dilation factor, defining the scaling of local update delays relative to the baseline cadence $\tau_0$.

#### Fundamental Relations

**1. Budget vs. Utilization**
The remaining budget $B(r)$ is inversely related to the local network utilization $U(r)$:
$$B(r) = 1 - U(r)$$
where $U(r)$ is the normalized node utilization ($U \to 0$ in flat, unstrained regions; $U \to 1$ at the limit of capacity saturation).

**2. Dimensionless Dilation**
The local dilation factor $\alpha(r)$ scales inversely with the remaining processing headroom:
$$\alpha(r) = \frac{1}{B(r)} = \frac{1}{1 - U(r)}$$
As utilization increases, the dilation factor diverges toward infinity, slowing down the rate of local state transitions.

**3. Dimensional Cadence**
The physical time interval $dt(r)$ required to complete a local node update is the product of the fundamental baseline tick $\tau_0$ and the local dilation factor:
$$dt(r) = \tau_0 \alpha(r) = \tau_0 \frac{1}{1 - U(r)}$$

#### The Unified Regime
Across all modeled scales, the local update timing is governed by the unified relation:
$$\alpha(r) = \frac{1}{1 - U(r)}, \quad dt(r) = \tau_0 \alpha(r)$$
This relation ensures that utilization $U(r)$ smoothly spans from quantum scale dynamics through the macroscopic gravitational transition, preventing mathematical divergences or step-function singularities across decades of distance.

#### The CaBS Action Principle
Physical wave patterns propagate through the node network along trajectories that extremize a functional of local dilation and processing budget under local strain constraints. This principle represents the network-level origin of least-action behavior, serving as the discrete foundation from which continuous geodesics and minimal-path principles emerge.

### TODO: Pattern-Rule Integration (See `SVET_issues_list.xls` — Tab “CaBS Rules”)

Future tasks:
*   Define explicit localized update rules for pattern motion, branching, stalling, and decay under CaBS dynamics.  
*   Verify via numerical simulation if these local rules naturally yield emergent geodesic paths.  
*   Validate the resulting propagation velocities against standard lattice simulations and audit configurations.

### 3.7 Operational Range of the Node Set

SVET dynamics operate within a finite, dimensionless excitation range that constrains all local update behavior, cadence scaling, and horizon formation. These bounds define the physically admissible region for node-level activity.

#### Axiom 1 — Excitation Norm
Define the local excitation as the dimensionless ratio:
$$\eta(x) = \frac{\rho_{\text{local}}(x)}{\rho_{\text{ref}}}$$
where the reference density $\rho_{\text{ref}}$ is taken as the Planck energy density. The admissible range is bounded as:
$$0 \le \eta \le 1$$
At minimal excitation, the node set's local value satisfies $\eta_{\text{vac}} \sim 10^{-122}$. This minimal excitation represents the local strain landscape (bias) created by the exactions of distant patterns propagating through the node set, rather than an active, self-sustained vacuum coherence.

#### Axiom 2 — Finite Update Capacity
Each node possesses a maximum update capacity $u_{\text{node,max}}$ defining the maximum number of coherent updates allowed per tick duration $\Delta t$ at Planck saturation ($\eta = 1$), constrained by the Margolus–Levitin limit:
$$u_{\text{node,max}} \sim \frac{2 E_{\text{ref}}\,\Delta t}{\pi \hbar}$$
where $E_{\text{ref}}$ is the energy in a reference node at saturation. The effective update rate scales linearly with local excitation:
$$u(\eta) = \eta\,u_{\text{node,max}}$$
This expresses the capacity-limited nature of the node set, directly linking local energy density, the update budget, and the discrete tick duration (distinct from the effective pattern-level cadence).

#### Axiom 3 — Collapse Bound for Extended Regions
While individual nodes may approach local saturation ($\eta \to 1$), extended regions cannot sustain uniform saturation. For a given region of radius $R$ containing $N$ nodes, the coarse-grained average excitation is defined as:
$$\bar{\eta} = \frac{1}{N}\sum_{i=1}^{N} \eta_i$$
There exists a critical excitation level $\eta_{\text{BH}}(R) \le 1$ such that if the average excitation exceeds this threshold, the region undergoes gravitational collapse, forming a local horizon:
$$\bar{\eta} > \eta_{\text{BH}}(R) \quad \Rightarrow \quad \text{horizon formation}$$
This bound distinguishes the microphysical saturation ceiling ($\eta = 1$) from the macroscopic, geometric boundary of black hole formation.

#### Axiom 4 — Tick Constraint (Nyquist Bound)
The discrete update tick $\Delta t$ must be short enough to resolve the highest physically relevant angular frequency $\omega_{\max}$ to prevent aliasing:
$$\Delta t \lesssim \frac{\pi}{\omega_{\max}}$$
If the Planck scale is taken as fundamental, the physical update rate cannot exceed the Planck time $t_P$, establishing the absolute limit:
$$t_P \le \Delta t \le \frac{\pi}{\omega_{\max}}$$
The tick selection governs representational resolution, while the local excitation $u(\eta)$ governs realized processing capacity; the two quantities are coupled but distinct.

#### Axiom 5 — Asymptotic Cadence Collapse
The node set never reaches a state of absolute, literal cessation of updates (literal zero-tick, or $\tau_{\text{eff}} = \infty$). Instead, as the local excitation approaches saturation ($\eta \to 1$), the effective cadence ($\tau_{\text{eff}}$) diverges asymptotically:
$$\lim_{\eta \to 1} \tau_{\text{eff}}(\eta) = \infty$$
Each incremental decimal increase in $\eta$ (e.g., $0.9 \to 0.99 \to 0.999$) requires exponentially higher local excitation densities, producing exponentially larger slowdowns in the local update cadence. This is a purely capacity-limited boundary condition: just as Special Relativity prevents massive particles from reaching $c$ through an exponential divergence of kinetic energy, SVET prevents the node set from reaching absolute temporal freezing through an exponential divergence of $\tau_{\text{eff}}$.

*Note on the Two-Layer Ontology:* Cadence collapse is strictly a pattern-level phenomenon. The underlying node set (the physical hardware) continues to respect the absolute, structural propagation limit $c$ (exactly one adjacency hop per network tick). What collapses under extreme excitation and routing cost is the capacity of extended, coherent patterns (the software) to exploit that raw network capacity. As local excitation approaches saturation ($\eta \to 1$), the effective pattern-level cadence diverges asymptotically, never reaching literal zero-tick, in the exact same manner that massive particle patterns asymptotically approach but never reach the invariant propagation rate $c$. In the weak-field limit, variations in $\tau_{\text{eff}}$ reproduce the gravitational redshift and time dilation of General Relativity, with $\tau_{\text{eff}}$ serving as the SVET analogue of the GR lapse function $g_{00}$, not as a dynamical metric component but as a pattern-level cadence field emerging from excitation [1]. This establishes the direct correspondence between SVET cadence and the GR lapse function $g_{00}$, ensuring that gravitational redshift emerges naturally from the excitation–cadence structure [1].

### 3.8 Coherence Manifold Mapping

The mapping from physical wave patterns to emergent metric geometry proceeds through a five-stage processing pipeline:

**1. Patterns to Strain**
Let the pattern be effectively represented as a local field $P(x)$ at macroscopic scales, which may consist of the wave function $\Psi(x)$ or a bundle of quantum fields. The strain tensor $S_{ij}(x)$ is an effective continuum representation of how the pattern stresses the local node set:
$$S_{ij}(x) = \mathcal{F}_{ij}\big[P(x), \partial_i P(x), \dots\big]$$
where the functional $\mathcal{F}_{ij}$ represents how the pattern's spatial profile stresses the local node set. Different components of $S_{ij}$ correspond to distinct physical channels (such as mass-like, charge-like, or spin-like strain). Under this mapping, $\Psi$ is placed as an input to the geometry-generation pipeline rather than being placed "inside" a pre-existing spacetime.

**2. Strain to Bias**
The accumulated strain tensor is mapped to a local bias field $B_a(x)$ defining the node set's directional update preferences:
$$B_a(x) = \mathcal{G}_a\big[S_{ij}(x)\big]$$
The functional $\mathcal{G}_a$ determines local update bias, representing the node-set-level origin of gravitational potentials, frame-dragging, and background biases ($B_0$).

**3. Bias to Local Coherence Cost**
The update bias defines a directional coherence cost density $C(x,v)$ for a pattern propagating through point $x$ with local direction vector $v$:
$$C(x,v) = \mathcal{H}\big(B_a(x), v\big)$$
This represents the local metric weight, defining how expensive it is in coherence terms to propagate a pattern along a given trajectory.

**4. Least-Cost Routing (Variational Principle)**
The trajectory $\gamma$ of a propagating pattern minimizes the total coherence action $A[\gamma]$:
$$A[\gamma] = \int_\gamma C(x, \dot{x})\,ds, \qquad \delta A[\gamma] = 0$$
Least-cost coherence routing paths are the geodesics of this cost functional.

**5. Metric Emergence**
If the cost function $C(x,v)$ is homogeneous of degree one in the velocity vector $v$, it can be modeled as a Finsler metric. Under isotropic assumptions, this reduces to a Riemannian metric tensor $g_{\mu\nu}(x)$ such that:
$$C(x,v) = \sqrt{g_{\mu\nu}(x)\,v^\mu v^\nu}$$
The emergent coherence manifold is $(M, g_{\mu\nu})$, where horizons and ergospheres represent critical, capacity-limited boundaries of the metric.

Because the emergent effective metric (pattern-level) $g_{\mu\nu}(x)$ determines routing cost $C(x,v)$ and local cadence, the excitation function $\eta(x)$ participates in a self-consistent routing cycle that shapes both geometry and propagation [1].

---

## 4. Flux Algebra

### 4.1 Flux as Directional Coherent Update Demand

In SVET, flux is not a field amplitude, probability wave, or abstract force carrier; rather, it is a **directional coherent update demand** propagated across the adjacent links of the node set. It represents a capacity-limited routing request from node $i$ to adjacent node $j$, tracking the transfer of coherent exaction states.

**Capacity Bounds**  
At any given tick, the coherent flux $F_{i\to j}$ from node $i$ to node $j$ is strictly bounded by both the available local budget headroom $B_i$ and the absolute physical update capacity $u(\eta_i)$ of the source node:
$$0 \le F_{i\to j} \le \min\big(B_i, u(\eta_i)\big)$$
This joint limit ensures that flux propagation remains bounded by the microphysical constraints of the local node set, preventing the build-up of unresolvable state demands.

**The Routing Request**  
Coherent flux is processed locally as an active accounting request. It does not exist independently of the node set; rather, it is a record of state-change requirements resolved locally through adjacency‑based ledger accounting between adjacent nodes.

### 4.2 Flux Addition and Cancellation

Superposition in SVET is governed by the vector addition and normalization of real-valued, directional coherent flux. Because phase is encoded purely through directional orientation and local cadence delays, wave interference behavior emerges directly from real-valued vector superposition.

**The Superposition Operator**  
When multiple flux demands $F_k$ converge on a single node, the resultant combined flux is resolved via a capacity-limiting normalization operator $\mathcal{N}$:
$$\vec{F}_{\text{tot}} = \mathcal{N}\left(\sum_{k} \vec{F}_k\right)$$
where $\mathcal{N}$ enforces that the total resultant flux remains within the local node's budget bounds.

**Directional Cancellation**  
Because flux vectors possess explicit physical orientations across adjacency links, cancellation occurs when opposing demands converge:
*   **Alignment (Constructive):** If $\vec{F}_1$ and $\vec{F}_2$ are parallel, their update demands reinforce each other, maximizing the resolved coherent flux.
*   **Opposition (Destructive):** If $\vec{F}_1 \approx -\vec{F}_2$, the opposing update demands cancel within the local ledger. The remaining unresolved portion of coherent update demand is diverted into the incoherent channel ($H$).

This vector-based subtraction replaces the standard wave mechanics requirement for complex probability amplitudes with real-valued, directional conservation bookkeeping.

### 4.3 Propagation, Reflection, and Refraction

The spatial paths of coherent update demands are governed by local capacity constraints and routing biases across the node set. These rule-driven resolutions produce the discrete behaviors of transmission, reflection, and refractive deflection.

**1. Coherent Transmission**  
Coherent propagation occurs when adjacent node $j$ has sufficient available budget $B_j$ to accept the incoming coherent demand $F_{i\to j}^{\text{eff}}$. The successfully transmitted fraction continues along its trajectory.

**2. Coherent Rejection (Reflection)**  
Reflection is a local ledger‑level rejection event. When the incoming effective flux exceeds the target node's available budget, the target node rejects the excess coherent demand. The unresolved portion remains coherent and is reflected back into the adjacency:
$$F_{i\to j}^{\text{refl}} = F_{i\to j}^{\text{eff}} - B_j \qquad \big(\text{when } F_{i\to j}^{\text{eff}} > B_j\big)$$

**3. Coherence Refraction**  
When propagating across regions of varying node strain, the trajectory of a wave-front is deflected. Because the local coherence cost $C(x,v)$ varies with the strain-induced bias $B_a(x)$, the pattern-level wave-front naturally bends toward directions of lower propagation cost. This discrete refraction reproduces Snell-like behavior in the continuum limit, serving as the local origin of emergent gravitational geodesics.

### 4.4 The Node Ledger (Conservation of Energy)

**Statement (operational):** Conservation of energy in SVET is a bookkeeping identity of the node-network update. Local update demand is partitioned at each node according to the success or failure of the pattern-dependent yield criterion and the local CaBS dynamics.

**Partition identity (node level):**

$$I_{\text{in}} = I_{\text{refl}} + I_{\text{trans}} + \Delta H$$

Equivalently, in normalized form:

$$R + T + H = 100\%$$

**Component definitions and locality**
- **$I_{\text{refl}}$ (Coherent Rejection / Reflection):** a *surface* event. Occurs when a neighbor node (or interface) cannot accept the incoming coherent demand; the rejected portion remains coherent and carries phase information away from the boundary.  
- **$I_{\text{trans}}$ (Coherent Propagation / Transmission):** the coherent portion successfully accepted by the neighbor and available for further coherent propagation.  
- **$\Delta H$ (Incoherent Energy / H):** a *bulk* event. Energy diverted into the incoherent channel when the pattern-dependent yield criterion is met (coherence $\to$ incoherence). $\Delta H$ is the local increment of incoherent energy that may later manifest as heat, photochemistry, fluorescence, photoemission, mechanical damage, etc.

**Link to yield and CaBS dynamics**  
The partition depends on the local budget $B$, pattern demand $S_p$, pattern stability $\Gamma_p$, and dynamic loading (CaBS) factors. In compact form:

$$
\text{Yield if}\quad \frac{S_p}{B}\,\Gamma_p\,\Phi(\dot S_p,\tau_{\text{eff}}) \ge \kappa_{\text{yield}}
$$

where $\Phi(\dot S_p,\tau_{\text{eff}})$ encodes rate/cadence dependence. If the yield condition is met at the node, the accepted coherent propagation fails and the corresponding energy is diverted into $\Delta H$; otherwise the ledger partitions into reflection and transmission according to local acceptance rules.

**Practical notes**
- **Surface vs bulk:** Always preserve the distinction in derivations and experiments: reflection is a boundary accounting event; H production is a bulk, post-acceptance event.  
- **Conservation semantics:** This identity is bookkeeping — energy is redistributed between coherent and incoherent channels; no external creation or destruction is invoked.  
- **Cross references:** See Sec. 2.6 (Incoherent Channel and Yield), Sec. 4.5 (Boundary Ledger and Tests), Sec. 11 (Computational Implementation) for logging and simulation protocols, and Sec. 13 (Predictions) for experimental tests.

*TODO:* Derive the partition identity from the node update algorithm and show how global conservation follows from local ledger reconciliation.


### 4.5 Boundary Ledger and Tests
**Note:** Boundary partitioning depends on the pattern-dependent yield criterion defined in Sec. 2.6 Incoherent Channel (H). See Sec. 4.4 The Node Ledger for the node-level partition identity and Sec. 11 Computational Implementation Layer for the simulation logging checklist used to validate boundary predictions.

**Summary**  
In SVET, boundary interactions are governed by local CaBS accounting. Incident coherent flux is partitioned at the surface into coherent reflection, coherent transmission, and incoherent bulk loss. Reflection is a surface accounting shock (coherent rejection), not a primary decoherence event. Decoherence (H) occurs only after coherent flux is accepted into the medium and then loses directional coherence.

**Boundary Ledger Identity**  
The local energy ledger at a boundary node satisfies:

$$I_{\text{in}} = I_{\text{refl}} + I_{\text{trans}} + I_{\text{heat}}$$

where:
- $I_{\text{refl}}$ is **coherent reflection** (surface event),  
- $I_{\text{trans}}$ is **coherent transmission** (accepted flux),  
- $I_{\text{heat}}$ is **incoherent bulk loss** (H channel).

**Local Acceptance Rule**  
For a boundary node with Budget $B$ and local Strain $S$, the instantaneous transmission fraction may be expressed as:

$$T \equiv \frac{I_{\text{trans}}}{I_{\text{in}}} \approx \frac{B}{B + S}$$

and the effective cadence (delay per update) is:

$$\tau_{\text{eff}} = \tau_0\left(1 + \left(\frac{S}{B}\right)^\beta\right)$$

These relations fix reflection and absorption once $B$ and $S$ are specified for the interface and bulk.

**Experimental Slab Test Specification (Normal Incidence)**

1. **Setup**  
   - Monochromatic source with known incident intensity $I_{\text{in}}$.  
   - Thin slab of material with well-characterized surface and bulk CaBS parameters $B_{\text{surf}}, S_{\text{surf}}, B_{\text{bulk}}, S_{\text{bulk}}$.  
   - Instruments: calibrated photodetectors for reflected and transmitted coherent intensity; calorimeter or bolometer for bulk heating $H$.

2. **Measurements**  
   - Measure $R = I_{\text{refl}}$, $T = I_{\text{trans}}$, and $H$ (energy deposited as incoherent channel).  
   - Verify ledger identity $R + T + H \approx I_{\text{in}}$ within experimental error.

3. **Predictions to test**  
   - Vary surface $B_{\text{surf}}$ (e.g., by coating) and observe predicted change in $R$ with $T$ and $H$ constrained by CaBS accounting.  
   - Under intense pumping, measure change in $S$ and resulting shifts in $T$ and $\tau_{\text{eff}}$ (pump-induced refractive index shifts).

4. **Controls**  
   - Use nonabsorbing reference (e.g., fused silica) to validate coherent reflection baseline.  
   - Use pump-probe to separate instantaneous coherent rejection from slower incoherent absorption dynamics.

**Simulation Logging Checklist**  
Record per node and per timestep:
- **Coherent flux vector** (magnitude and orientation)  
- **Local B, S, \tau_eff**  
- **I_refl, I_trans, \Delta H** (energy moved into incoherent channel)  
- **Phase coherence metric** (e.g., vector alignment index)  
- **Boundary ledger reconciliation events** (rejection vs acceptance)

**Cross-references**  
- Cross-reference this subsection in **Section 5 (Emergent Wave Mechanics)** for interference consequences.  
- Cross-reference in **Section 10 (Material Response & Dispersion)** for mapping H to material observables.  
- Cross-reference in **Section 12 (Predictions)** for experimental claims.  
- Refer to **Section 11 (Computational Implementation)** for logging and simulation details.

*TODO: Establish a qualitative definition for a strain-cost functional. This functional will assign a numerical cost to a pattern’s attempt to propagate across a node and its adjacent neighbors based on local update demands. Rather than prematurely committing to a specific variational mathematical form, this placeholder serves to develop how spatial-temporal propagation paths (geodesics) minimize total network-level strain.*

### 4.6 Energy as Update Demand

In SVET, energy is not a substance, not a field excitation, and not a quantity stored in objects. Energy is the update demand a pattern imposes on the node set. Every pattern is a coherence-preserving configuration that must be locally resolved under the update rule at each tick. The more intricate the pattern's internal structure or the stronger its directional persistence, the greater the update demand required to maintain it. Energy is the measure of this demand.

The node set does not supply, store, or transfer energy. The same adjacency-preserving update rule applies uniformly across the node set. A pattern with high oscillatory complexity or strong directional persistence requires a higher update demand under the same rule to maintain identity across ticks. This update demand is resolved by the update rule against the local budget; energy is the node-set-level accounting of the pattern's exaction demand [1].

This reframes kinetic and potential energy.  

**Kinetic energy** is the increased update demand associated with strong directional persistence: the requirement that the pattern be resolved in a way that preserves a persistent direction of propagation.  

**Potential energy** is the update demand associated with a pattern's position within a cadence gradient ($\nabla \tau_{\text{eff}}$) — regions where the local resolution latency $\Delta\tau(x)$ differs from the baseline [1]. Changes in local update demand across a cadence gradient are balanced by local cadence-suppression adjustments and coherence-shedding ($\Delta H$), ensuring no loss of ledger identity [1]. Both forms of energy are expressions of the same principle: the cost of maintaining coherence under the local update rules.

Because the node set cannot store energy, conservation of energy becomes conservation of coherence constraints. Unresolved exaction is diverted into the incoherent channel $\Delta H$, ensuring no local accumulation [1]. When patterns interact, their combined update demands must reconcile into a configuration that preserves the total exaction demand; inelastic interactions divert the unrecoverable portion into the incoherent channel as the Decoherence Tax ($\Delta H$) [1]. No energy is transferred; the exaction-driven coherence constraints are redistributed. Conservation is exact because the node set has no mechanism to absorb or erase coherence constraints.

Energy is therefore not a thing a pattern possesses. It is a constraint: the requirement that a pattern maintain coherence across a flat, uniform, adjacency-preserving node set. Patterns with greater update demand behave as if they "have more energy," but this is simply the same local update rules resolving a more demanding pattern. Energy is the cost of coherence.

### 4.7 Momentum as Directional Coherence

In SVET, momentum is not a quantity carried by an object, nor a conserved vector stored in space. Momentum is the instantaneous directional asymmetry of a pattern's local strain footprint within a single frozen tick. This asymmetry compels the update rule to resolve the pattern along a persistent direction on the next tick. A pattern with strong directional asymmetry exhibits a stable propagation direction because its internal structure exacts it [1].

Every pattern expresses a single coherence-constraint set that preserves its identity, oscillation, phase, and directional asymmetry within each tick [1]. The update rule does not push patterns forward; it resolves their exaction demands uniformly across adjacency. A pattern with strong directional asymmetry exacts the update rule to resolve it in a way that maintains its direction. This directional asymmetry is what SVET identifies as momentum [1].

Momentum is therefore not a force, not a stored quantity, and not a property of space. It is a coherence constraint internal to the pattern. A pattern with high directional asymmetry resists changes to its coherence-minimal propagation path because altering direction would require reconfiguring its coherence constraints [1]. This resistance is what we interpret as inertia.

As a pattern's directional asymmetry approaches the adjacency-hop limit, its local strain footprint becomes increasingly anisotropic, driving its update demand toward the saturation ceiling ($U \to 1$). This produces the observed relativistic momentum scaling without invoking mass increase or geometric curvature.

When patterns interact, their directional coherence constraints must reconcile into a configuration that preserves the total exaction demand. The update rule does not transfer momentum; it enforces coherence consistency. Inelastic interactions divert unrecoverable directional coherence into the incoherent channel $\Delta H$ as directional decoherence [1].

This reframes collisions and interactions. When two patterns meet, their directional asymmetry profiles and coherence constraints combine, distort, or redistribute [1]. The resulting coherence-minimal continuation path is the one that satisfies the coherence constraints of both patterns while preserving total update demand. No momentum is "exchanged"; instead, directional coherence is reallocated, with any unrecoverable portion shed into $\Delta H$ [1].

Momentum is not something a pattern has. It is something a pattern is doing: maintaining directional asymmetry under the invariant adjacency-preserving update rule [1]. Momentum is the persistence of its coherence-minimal propagation path.

### 4.8 Conservation as Coherence-Constraint Accounting

In SVET, conservation laws do not arise from spacetime symmetries or from fields storing and transferring quantities. Conservation emerges from a simpler and more fundamental requirement: patterns must maintain coherence across discrete ticks under the update rule. The node set does not store energy, momentum, or information. The invariant adjacency-preserving update rule resolves exaction demands uniformly across adjacency. Because the node set has no mechanism to absorb or erase coherence constraints, all coherence must be accounted for during interactions. This is the SVET meaning of conservation.

Every pattern expresses a single coherence-constraint set that preserves its identity, oscillation, phase, and directional asymmetry within each tick. When patterns interact, their coherence constraints must reconcile into a new configuration that preserves the total ledger identity. Total conservation refers to the full node-ledger identity:
$$I_{\text{in}} = I_{\text{refl}} + I_{\text{trans}} + \Delta H = 100\%$$
which includes coherent exaction, reflected exaction, transmitted exaction, and the incoherent channel $\Delta H$. Coherence constraints are redistributed among the resulting patterns, with any unrecoverable portion diverted into $\Delta H$ as decoherence. Conservation is therefore not an imposed physical law but the logical consequence of maintaining pattern identity under the update rule.

This reframes traditional conserved quantities.  
**Energy conservation** becomes the preservation of total update demand across the full ledger identity.  
**Momentum conservation** becomes the preservation of total directional asymmetry across the ledger [1].  
Higher-order conserved quantities (such as phase-encoded pattern symmetries) emerge only after the pattern taxonomy is introduced in Chapter 5.

Interactions are not exchanges of physical quantities but reconfigurations of coherence constraints. When two patterns meet, their internal coherence constraints and directional asymmetry combine, distort, or redistribute into new patterns whose total ledger identity matches the original. The update rule does not transfer quantities; it deterministically resolves all exaction demands all exaction demands under the same invariant adjacency-preserving rule. Conservation emerges because the update rule enforces exact ledger consistency at every tick.

In SVET, conservation is not a property of matter or fields. It is a property of coherence accounting in a universe where patterns must maintain identity across a flat, adjacency-preserving node set. Conservation is the unavoidable consequence of coherence-constraint continuity.

### 4.9 Forces as Coherence-Gradient Responses

In SVET, forces are not pushes or pulls transmitted through fields, nor are they interactions mediated by particles. A force is the behavior of a pattern maintaining coherence in the presence of a non-uniform cadence environment. The node set does not generate forces; the invariant adjacency-preserving update rule resolves exaction demands uniformly across adjacency. What appears as a force is the pattern's coherence-preserving response to local cadence gradients.

Every pattern expresses a single coherence-constraint set that preserves its identity, oscillation, phase, and directional asymmetry within each tick. When the local cadence is uniform, a pattern follows a coherence-minimal continuation path because this path requires no reconfiguration of its directional asymmetry. When the cadence varies—due to nearby patterns, accumulated update demand, or a local cadence suppression gradient—the coherence-minimal continuation path is no longer unbiased. The pattern must adjust its propagation to remain coherence-consistent with the local cadence gradient. This adjustment is interpreted macroscopically as a force.

A cadence gradient is an adjacency-indexed variation in resolution latency $\Delta\tau(x)$ and effective cadence $\tau_{\text{eff}}(x)$, driven by local utilization $U(x)$ [1]. A force is therefore not something acting on a pattern. It is the requirement that the pattern maintain coherence under changing local constraints. A pattern with strong directional asymmetry resists changes to its coherence-minimal continuation path, which manifests as inertia. A pattern in a steep cadence gradient must adopt a deflected coherence-minimal continuation path, which manifests as acceleration. The update rule does not cause these behaviors; it enforces coherence consistency at each node tick [1].

This reframes classical forces.  
**Gravitational attraction** becomes the tendency of patterns to follow coherence-minimal continuation paths in regions where cadence gradients arise from accumulated update demand.  
**Electromagnetic forces** arise from phase-coherence relationships between patterns that modify local cadence structure.  
**Nuclear forces** emerge from extreme coherence-density conditions where only tightly constrained coherence configurations remain stable.  
In all cases, the node set plays no active role; the apparent force is the pattern's coherence-preserving response to local cadence conditions.

Because the node set cannot store or transmit forces, all interactions are Coherence-Constraint Resolutions enforced by the adjacency-preserving update rule. When patterns present overlapping adjacency demands on neighboring nodes, their coherence constraints enter a configuration in which not all constraints can be simultaneously satisfied [1]. The update rule resolves this configuration into a new arrangement of coherence-constraint sets, preventing the need for force-carrying mediator particles. Inelastic deflections shed unrecoverable coherence into the incoherent channel $\Delta H$ as directional decoherence [1]. No quantity is exchanged; the patterns simply follow the coherence-minimal continuation paths that resolve their joint constraints.

In SVET, forces are not fundamental entities. They are emergent behaviors arising from the requirement that patterns maintain coherence in a node set whose cadence structure is shaped by other patterns. Forces are coherence-gradient responses.

### 4.10 Acceleration as Coherence-Strain Minimization

In SVET, acceleration is not caused by forces acting on objects, nor by curvature of spacetime. Instead, acceleration is the pattern-level adjustment of its coherence-minimal continuation path in response to variations in local cadence and coherence strain. The node set does not push, pull, bend, or curve anything; the invariant adjacency-preserving update rule resolves exaction demands uniformly across adjacency.

Every pattern expresses a single coherence-constraint set whose directional asymmetry biases how it is resolved within each tick. In a uniform cadence environment, the coherence-minimal continuation path is strain-minimal (traditionally interpreted as straight-line motion). When local cadence varies—due to nearby patterns, accumulated update demand, or a local cadence suppression gradient—the previously strain-minimal continuation path no longer preserves the coherence-constraint set. The pattern's continuation path deflects to minimize coherence strain. This deflection is what appears macroscopically as acceleration.

A cadence gradient is an adjacency-indexed variation in resolution latency $\Delta\tau(x)$ and effective cadence $\tau_{\text{eff}}(x)$, driven by local utilization $U(x)$. A pattern with strong directional asymmetry resists changes to its continuation path, which manifests as inertia. When cadence gradients become sufficiently steep, the strain-minimal continuation path deflects, and the pattern follows that deflection automatically. No force is transmitted; no field mediates the interaction. The deflection is the pattern's own coherence-preservation requirement.

Gravitational acceleration arises when a pattern encounters a region where $\Delta\tau(x)$ increases (cadence suppression) [1]. The coherence-minimal continuation path deflects toward regions of higher cadence-suppression gradient [1]. The pattern accelerates not because it is pulled, but because maintaining its previous continuation path would violate its coherence-constraint set [1].

Electromagnetic acceleration follows the same principle. Phase-coherence asymmetries between patterns create localized cadence suppression. Patterns adjust their continuation paths to minimize coherence strain relative to these phase relationships. No field or mediator is required.

Inelastic acceleration sheds unrecoverable directional coherence into the incoherent channel $\Delta H$ as directional decoherence [1]. Because the node set cannot store or transmit forces, all acceleration is an emergent consequence of coherence-constraint preservation in a flat, adjacency-preserving node set. Acceleration is the operational expression of strain-minimal continuation under non-uniform cadence conditions.

### 4.11 Interaction as Coherence-Constraint Resolution

In SVET, interactions are not collisions between objects, nor are they exchanges of particles or field-mediated forces. Interactions arise when multiple coherence-constraint sets simultaneously request re-instantiation within the same adjacency neighborhood. When overlapping adjacency demands drive the local utilization:
$$U(x) = \frac{S(x)}{B}$$
toward the saturation ceiling ($U \to 1$), the local lattice strain $S(x)$ inflates. Because the node set cannot exceed its capacity, the update rule must resolve these conflicting exaction requests into a configuration that preserves coherence across successive node ticks under the invariant local update rules [1].

Every pattern expresses a single coherence-constraint set that preserves its identity, oscillation, phase, and directional asymmetry within each tick. When patterns present overlapping adjacency demands on neighboring nodes, their coherence-constraint sets enter a configuration in which not all constraints can be simultaneously satisfied. The adjacency-preserving update rule resolves this configuration into a new arrangement of coherence-constraint sets that preserves the full ledger identity:
$$I_{\text{in}} = I_{\text{refl}} + I_{\text{trans}} + \Delta H = 100\%$$
This rule-driven resolution is the SVET meaning of interaction.

The node set does not coordinate or mediate this process; it simply resolves all exactions under the same invariant local update rule everywhere. Because the node set cannot absorb coherence, the combined coherence-constraint set must be conserved across the ledger. Patterns cannot offload coherence into the node set [1]. Instead, the update rule resolves their overlapping constraints into new coherence-constraint configurations. These resolved configurations appear experimentally as scattering, shared coherence-minimal continuation paths, divergent continuation paths, or the formation of new stable patterns.

This reframes the idea of "force carriers." In SVET, there are no mediating particles. What we call a "force" is the deflection of the coherence-minimal continuation path that emerges from constraint resolution. Patterns with incompatible phase-coherence relationships undergo divergent continuation because maintaining coherence requires separation. Patterns with compatible phase-coherence relationships adopt shared continuation solutions because the coherence-minimal configuration is a jointly satisfied constraint set.

Patterns that appear to annihilate do not disappear. In annihilation-like resolutions, the rigidity of the original coherence-constraint sets collapses, and their update demand is reallocated into high-cycle phase-oscillation patterns. This is the SVET mechanism for matter-to-radiation conversion, preserving the full ledger identity. Inelastic interactions shed unrecoverable coherence into the incoherent channel $\Delta H$ as directional decoherence.

Because the node set cannot store or transmit interaction effects, all interactions are local coherence-constraint resolutions. The apparent strength of an interaction corresponds to how severely the patterns' coherence constraints conflict [1]. Strong interactions arise when coherence-constraint sets are highly rigid and cannot be jointly satisfied without major reconfiguration. Weak interactions arise when constraint sets can be jointly satisfied with minimal coherence strain.

In SVET, interaction is not a fundamental process. It is the emergent behavior of coherence-constraint sets being resolved by the adjacency-preserving update rule while sharing the same adjacency neighborhood of a flat, fixed node set. Interaction is coherence-constraint resolution.

### 4.12 Mass as Resistance to Coherence-Constraint Reconfiguration

In SVET, mass is not an intrinsic property of matter, nor a coupling to a Higgs field, nor a measure of stored energy. Mass is the resistance a pattern exhibits when its coherence-constraint set is required to reconfigure under cadence-indexed update pressure [1]. Because patterns must maintain coherence within each tick of a flat, adjacency-preserving node set, any change to their coherence-minimal continuation path requires a reconfiguration of their internal and directional constraints. The degree of resistance to this reconfiguration is what appears experimentally as mass.

Every pattern expresses a specific coherence-constraint set: a stable arrangement of oscillation, phase relationships, and directional asymmetry. Some patterns have tightly constrained coherence-constraint sets that cannot be altered without violating identity. These patterns exhibit high resistance to changes in their continuation path and therefore appear to have high mass. Other patterns have more flexible constraint sets that can be reconfigured with minimal coherence strain, appearing to have low mass.

Mass is therefore not a substance or a field interaction. It is a measure of coherence rigidity. A pattern with high mass is one whose coherence-constraint set strongly resists reconfiguration. A pattern with low mass is one whose constraint set can adapt more easily. The node set does not impose mass; it enforces coherence continuity. Mass emerges from the internal structure of the coherence-constraint set itself and its resistance to reconfiguration under the local cadence suppression gradient $\nabla \tau_{\text{eff}}(x)$ and utilization $U(x)$.

This reframes inertia. Inertia is the resistance of a coherence-constraint set to altering its directional asymmetry. A pattern with high mass requires significant constraint reconfiguration to change its continuation path, so it accelerates slowly. A pattern with low mass requires minimal reconfiguration, so it accelerates easily. The node set does not push or pull; it resolves exaction requests according to the same adjacency-preserving update rule everywhere.

Mass also reframes gravitational behavior. In a cadence suppression gradient, patterns must adjust their continuation paths to remain coherence-consistent. Although a high-mass pattern resists internal reconfiguration more strongly, the coherence-minimal continuation path is determined entirely by the local cadence suppression gradient $\nabla \tau_{\text{eff}}(x)$, not by the pattern's rigidity [1]. Under the Single-Tick Identity Principle (STIP), all patterns evaluate the same adjacency-local latency structure, so they follow the same deflected continuation path. The Equivalence Principle emerges because the least-strain continuation is an absolute property of the local update-latency landscape, not of the pattern.

Mass should not be confused with material hardness or melting point. Mass reflects the internal rigidity of a single pattern's coherence-constraint set, while hardness and melting point reflect the rigidity of many patterns arranged in a shared adjacency configuration [1]. A material such as lead can contain high-mass patterns yet remain soft because its multi-pattern constraint configuration is easily reconfigured [1]. Titanium appears hard not because its patterns have greater mass, but because its multi-pattern constraint configuration is highly resistant to reconfiguration [1].

Melting behavior follows the same principle. A solid crystal is a repeating multi-pattern configuration whose coherence-constraint sets must be jointly satisfied across a shared adjacency neighborhood. Heating is the injection of non-directional update strain that drives the local utilization $U(x)$ toward the saturation ceiling. A loosely constrained multi-pattern configuration reaches a point where the rising utilization overwhelms its ability to maintain constraint continuity, forcing a coherence failure in which the shared adjacency instructions are rejected and diverted into the incoherent channel as coherence-shedding $\Delta H$ [1]. A tightly constrained configuration can tolerate far more utilization before this failure occurs, producing a high melting point [1].

These distinctions show that mass, hardness, and melting point are not different physical categories but different structural scales of coherence-constraint rigidity: internal rigidity for mass, multi-pattern rigidity for hardness, and constraint-configuration failure thresholds for melting [1].

Because the node set cannot store or transmit mass, mass is always a pattern-internal coherence rigidity. It is not transferred, exchanged, or mediated. When patterns present overlapping adjacency demands on neighboring nodes, their coherence-constraint sets are resolved into new patterns whose apparent mass reflects the rigidity of the resulting constraint set. Under the node ledger identity,
$$I_{\text{in}} = I_{\text{refl}} + I_{\text{trans}} + \Delta H = 100\%,$$
the total rest-mass complexity may be converted into high-frequency instantiation trajectories (radiation) or incoherent jitter $\chi$, but no update demand is ever lost.

In this view, mass is not fundamental. It is the emergent measure of how difficult it is to reconfigure a coherence-constraint set while preserving identity within each tick. Mass is coherence rigidity.

### 4.12 Mass as Resistance to Coherence-Constraint Reconfiguration

In SVET, mass is not an intrinsic property of matter, nor a coupling to a Higgs field, nor a measure of stored energy. Mass is the resistance a pattern exhibits when its coherence-constraint set is required to reconfigure under cadence-indexed update pressure [1]. Because patterns must maintain coherence within each tick of a flat, adjacency-preserving node set, any change to their coherence-minimal continuation path requires a reconfiguration of their internal and directional constraints. The degree of resistance to this reconfiguration is what appears experimentally as mass.

Every pattern expresses a specific coherence-constraint set: a stable arrangement of oscillation, phase relationships, and directional asymmetry. Some patterns have tightly constrained coherence-constraint sets that cannot be altered without violating identity. These patterns exhibit high resistance to changes in their continuation path and therefore appear to have high mass. Other patterns have more flexible constraint sets that can be reconfigured with minimal coherence strain, appearing to have low mass.

Mass is therefore not a substance or a field interaction. It is a measure of coherence rigidity. A pattern with high mass is one whose coherence-constraint set strongly resists reconfiguration. A pattern with low mass is one whose constraint set can adapt more easily. The node set does not impose mass; it enforces coherence continuity. Mass emerges from the internal structure of the coherence-constraint set itself and its resistance to reconfiguration under the local cadence suppression gradient $\nabla \tau_{\text{eff}}(x)$ and utilization $U(x)$.

This reframes inertia. Inertia is the resistance of a coherence-constraint set to altering its directional asymmetry. A pattern with high mass requires significant constraint reconfiguration to change its continuation path, so it accelerates slowly. A pattern with low mass requires minimal reconfiguration, so it accelerates easily. The node set does not push or pull; it resolves exaction requests according to the same adjacency-preserving update rule everywhere.

Mass also reframes gravitational behavior. In a cadence suppression gradient, patterns must adjust their continuation paths to remain coherence-consistent. Although a high-mass pattern resists internal reconfiguration more strongly, the coherence-minimal continuation path is determined entirely by the local cadence suppression gradient $\nabla \tau_{\text{eff}}(x)$, not by the pattern's rigidity [1]. Under the Single-Tick Identity Principle (STIP), all patterns evaluate the same adjacency-local latency structure, so they follow the same deflected continuation path. The Equivalence Principle emerges because the least-strain continuation is an absolute property of the local update-latency landscape, not of the pattern.

Mass should not be confused with material hardness or melting point. Mass reflects the internal rigidity of a single pattern's coherence-constraint set, while hardness and melting point reflect the rigidity of many patterns arranged in a shared adjacency configuration [1]. A material such as lead can contain high-mass patterns yet remain soft because its multi-pattern constraint configuration is easily reconfigured [1]. Titanium appears hard not because its patterns have greater mass, but because its multi-pattern constraint configuration is highly resistant to reconfiguration [1].

Melting behavior follows the same principle. A solid crystal is a repeating multi-pattern configuration whose coherence-constraint sets must be jointly satisfied across a shared adjacency neighborhood. Heating is the injection of non-directional update strain that drives the local utilization $U(x)$ toward the saturation ceiling. A loosely constrained multi-pattern configuration reaches a point where the rising utilization overwhelms its ability to maintain constraint continuity, forcing a coherence failure in which the shared adjacency instructions are rejected and diverted into the incoherent channel as coherence-shedding $\Delta H$ [1]. A tightly constrained configuration can tolerate far more utilization before this failure occurs, producing a high melting point [1].

These distinctions show that mass, hardness, and melting point are not different physical categories but different structural scales of coherence-constraint rigidity: internal rigidity for mass, multi-pattern rigidity for hardness, and constraint-configuration failure thresholds for melting [1].

Because the node set cannot store or transmit mass, mass is always a pattern-internal coherence rigidity. It is not transferred, exchanged, or mediated. When patterns present overlapping adjacency demands on neighboring nodes, their coherence-constraint sets are resolved into new patterns whose apparent mass reflects the rigidity of the resulting constraint set. Under the node ledger identity,
$$I_{\text{in}} = I_{\text{refl}} + I_{\text{trans}} + \Delta H = 100\%,$$
the total rest-mass complexity may be converted into high-frequency instantiation trajectories (radiation) or incoherent jitter $\chi$, but no update demand is ever lost.

In this view, mass is not fundamental. It is the emergent measure of how difficult it is to reconfigure a coherence-constraint set while preserving identity within each tick. Mass is coherence rigidity.

### 4.14 Instantiation Trajectory and Instantiation Routing

SVET distinguishes between the pattern's identity-encoded one-hop adjacency instruction and the node set's realized adjacency resolution. These two constructs describe different projections of the same single-tick update operation and must not be conflated [1].

#### 4.14.1 Instantiation Trajectory (Pattern-Side Request)

A pattern does not store a worldline, a velocity, or a multi-tick plan. Its coherence-constraint set encodes a one-hop adjacency instruction: the next adjacency offset implied by the pattern's frozen-tick identity, independent of local budget, utilization, or cadence suppression [1]. This instruction is part of the identity and represents the pattern's internal adjacency demand [1].

This request is:
- identity-encoded,
- local,
- unconstrained by budget or strain,
- and not guaranteed to be realized.

It is not motion; it is the structurally implied next adjacency encoded in the pattern's coherence-constraint set [1].

#### 4.14.2 Instantiation Routing (Node-Set Resolution)

The node set performs the actual instantiation. On each tick, the node set resolves the pattern's one-hop adjacency instruction using its local strain $S(x)$, utilization $U(x)$, and cadence suppression gradient $\nabla \tau_{\text{eff}}(x)$ [1]. The result is the realized adjacency hop, determined entirely by the least-strain resolution of the local ledger.

Routing is:
- external,
- constrained,
- deterministic,
- and physically realized.

It is not the pattern's request; it is the executed next adjacency [1]. If the node set cannot satisfy the full adjacency instruction, the unrecoverable remainder is shed into the incoherent channel $\Delta H$.

#### 4.14.3 The Frozen-Tick Handshake

The frozen tick contains both:
1.  the pattern's one-hop adjacency instruction (trajectory), and  
2.  the node's local budget, utilization, and cadence-suppression constraints (routing conditions) [1].

Together, these determine the next tick's instantiation. No additional temporal information is stored or permitted. Under the Single-Tick Identity Principle (STIP), Layer 2 does not persist across ticks; the pattern is reconstructed each tick by Layer 1.

#### 4.14.4 Layer Interaction Summary
*   **Layer 2** provides the identity-encoded adjacency request.  
*   **Layer 1** resolves the request and reconstructs the pattern.  
*   Motion emerges from differences between ticks, not from stored trajectories.  
*   Identity remains frozen; routing is the realized update.

This separation preserves locality, discreteness, and the no-geometry, no-field ontology of SVET.

### 4.15 The Single-Tick Identity Principle (STIP)

SVET models the vacuum strictly as a static, non-coordinate node set governed by local update rules. To preserve the two-layer ontology and prevent continuous-field or geometric drift, STIP establishes the absolute mathematical boundary of pattern-level representation.

#### The Frozen Tick as an Evaluation Frame

The term "frozen tick" does not imply that the node set halts or that time stops. It is a conceptual evaluation frame used to analyze the static ledger state between updates. Nodes do not freeze; ticks define the discrete temporal boundaries at which identity is evaluated independently of motion. Motion emerges only from differences between ticks.

#### Axiom 1 — Non-Simultaneous Operations

A pattern's internal update cycle (frequency and phase-cycling) and its external translation (realized adjacency changes) are not parallel physical processes. They are distinct operational parameters encoded in the same Layer 2 instruction packet and resolved sequentially by the single, invariant local update rule of the node set.

#### Axiom 2 — Asymptotic Cadence Limit

The node set remains static and does not perform background updates in empty space. All physical "work" of state updates is performed when the node set expends its local capacity to honor a pattern's exaction. As the local utilization approaches saturation,
$$U(x) = \frac{S(x)}{B} \to 1$$
the effective pattern-level cadence diverges asymptotically. It never reaches a literal zero-tick rate, just as massive patterns asymptotically approach but never reach the invariant propagation rate $c$ [1].

#### Statement of the Law

A pattern's complete physical identity at any single-tick evaluation frame is fully encoded in the static configuration of the node set. This conceptual slice contains:
- the pattern's coherence-constraint set (identity),
- the local asymmetric strain footprint (momentum bias),
- the one-hop adjacency-offset instruction (next-tick request).

No additional temporal information is stored, required, or permitted.

#### Corollary 1 — No Multi-Tick Storage

A pattern does not store a trajectory, worldline, phase history, velocity, or acceleration. All such quantities arise exclusively from differences between ticks. Layer 2 does not persist across ticks; it is reconstructed each tick by Layer 1.

#### Corollary 2 — Local Determinism

The next tick's instantiation is fully determined by the local handshake between:
- the pattern's one-hop adjacency instruction, and
- the node's local strain, budget, utilization, and cadence-suppression state.

No non-local information participates in the update. If the node set cannot satisfy the full adjacency instruction, the unrecoverable remainder is shed into the incoherent channel $\Delta H$ [1].

#### Corollary 3 — Identity Completeness

The frozen tick contains the full identity of the pattern, including:
- mass (constraint-set rigidity),
- inertia (reconfiguration cost),
- spin (adjacency-offset symmetry),
- frequency class (cyclic adjacency pattern),
- momentum bias (strain asymmetry),
- the next immediate adjacency request.

#### Corollary 4 — No Future Prediction

The frozen tick contains exactly one shift-indexed tick's worth of forward information: the next adjacency request. Nothing beyond this is encoded or permitted.

#### Forensic Role

STIP enforces:
*   strict locality,
*   discreteness,
*   a non-coordinate, non-geometric ontology,
*   a no-field ontology,
*   a non-agency node set,
*   and the strict separation between identity and motion.

#### Interpretive Summary

Identity is frozen.  
Motion is the difference.  
Trajectory is the realized sequence of instantiation routings.  
Physics is the ledger resolving one tick at a time.

### 4.16 Singularities, Coherence-Catastrophe, and the Cadence Suppression Gradient

SVET does not permit geometric singularities. The node set is flat, adjacency-preserving, and cannot collapse, compress, or form infinities. What fails in extreme-density regimes is not the node set, but the capacity threshold of pattern-level coherence reconstruction [1].

A pattern's identity exists only as an instantaneous, tick-indexed coherence-constraint configuration resolved locally under the update rule. As exaction density increases, the local utilization ratio:
$$U(x) = \frac{S(x)}{B}$$
approaches the non-reducible Planck Saturation Ceiling ($U \to 1$). At this limit, the effective reconstruction cadence $\tau_{\text{eff}}(x)$ grows without bound. The local resolution latency $\Delta \tau(x)$ increases asymptotically; updates slow arbitrarily but never reach zero, ensuring that pattern-level reconstruction remains locally resolvable at extended tick intervals.

When $U$ reaches the saturation limit, the local update rules can no longer satisfy the pattern's coherence constraints. This is **Coherence-Catastrophe**: the pattern's coherence-constraint configuration fails, and the unresolved exaction load is diverted into the incoherent channel as a local coherence-shedding increment $\Delta H$ [1]. This channel represents non-patternized node-set jitter $\chi$ [1], the native mechanism for decoherence and entropy increase.

Because cadence never fully halts, $\Delta H$ is not trapped. It diffuses outward through adjacency-indexed jitter redistribution over extended tick intervals [1]. No infinite stacking occurs, because the node ledger enforces a strict **Accounting Shock** boundary at $U = 1$: no further coherent exaction can be accepted at that saturated site.

#### The Cadence Suppression Gradient

The **Cadence Suppression Gradient** is the adjacency-indexed variation in effective reconstruction cadence $\tau_{\text{eff}}(x)$ that naturally forms around a high-density core. It is not geometric curvature; it is a local update-latency landscape induced by differential exaction load [1].

It has three structural consequences:

**1. Continuation Bias**  
As successive adjacency instantiations occur under varying cadence, patterns follow continuation paths that minimize local coherence cost [1]. This differential reconstruction delay produces the emergent macroscopic behavior historically interpreted as gravitational redshift, lensing, and time dilation.

**2. Coherence Horizon (One-Way Gate)**  
The gradient extends outward from the Planck core. The **Coherence Horizon** is the causal boundary where the cadence gradient becomes steep enough that outward adjacency-coherent instantiation cannot be resolved [1].  
*   Inward continuation instantiates normally.  
*   Outward adjacency-coherent continuation fails.  
*   No coherence-catastrophe occurs at the horizon.

**3. Horizon-Level Evaporation**  
Evaporation occurs at the horizon boundary, not at the core. The boundary is where the extended gradient's local strain interacts with the Local Floor Budget $B_0(x)$ of the surrounding vacuum [1]. This produces outward redistribution of $\Delta H$ without requiring cross-horizon transport from the core.

**3. Horizon-Level Evaporation**  
Evaporation occurs at the horizon boundary, not at the core. The boundary is where the extended gradient's local strain interacts with the Local Floor Budget $B_0(x)$ of the surrounding vacuum [1]. This produces outward redistribution of $\Delta H$ without requiring cross-horizon transport from the core [1].

#### Unified Interpretation

*   The Planck core is the only region where $U = 1$ and Coherence-Catastrophe occurs [1].  
*   The horizon is a one-way causal gate created by the cadence suppression gradient.  
*   The gradient itself replaces geometric curvature and ensures:
    *   no region ever halts its processing loop,  
    *   no infinite stacking occurs,  
    *   and horizon-level evaporation emerges naturally from adjacency-indexed cadence-suppression gradients [1].  

Singularities are therefore **finite coherence-catastrophe zones**, not geometric infinities.

### 4.x Architectural Correspondence: Classical Quantities as SVET Coherence Primitives

To connect SVET’s coherence-based ontology with the familiar quantities of classical and quantum physics, three structural correspondences can be identified. These are not additional assumptions layered onto the node set; they emerge directly from the local accounting of update demand and coherence constraints.

**Rest Mass ($m$):**  
In SVET, mass is not an intrinsic substance or stored quantity. It is the stationary update demand of a pattern — the persistent exaction required to maintain its internal coherence across node ticks. A stationary pattern authorizes a stable, localized update cost, producing the effective cadence lag associated with rest mass.

**Momentum ($p$):**  
Momentum is not a conserved vector carried by an object. It is the directional coherence of a pattern — the requirement that its re-instantiation across ticks preserve a persistent direction. Patterns with strong directional coherence resist changes to their coherence-minimal propagation path, giving rise to the phenomenon interpreted as inertia.

**Conservation Laws:**  
Conservation does not arise from continuous spacetime symmetries. It follows from the node set's inability to absorb or erase coherence constraints. During interactions, total update demand, total directional coherence, and total phase asymmetry must remain constant. Conservation is therefore the exact continuity of coherence constraints across discrete node ticks.

**Inertia as Coherence Reconfiguration Cost:**  
In SVET, a pattern resists changes to its direction because altering its propagation requires reconfiguring its internal coherence. A pattern with strong directional coherence maintains a stable propagation direction across node ticks, and any deviation from that direction demands a restructuring of its coherence constraints. This structural resistance to reconfiguration is what manifests macroscopically as inertia.

**Momentum Without Exchange:**  
Traditional physics treats collisions as exchanges of momentum between objects. In SVET, no quantity is transferred. When patterns interact, their coherence constraints must reconcile into a configuration that preserves total update demand and total directional coherence. The resulting propagation paths are the coherence‑minimal solutions that satisfy both patterns’ constraints. Momentum conservation emerges not from exchange, but from the Node Set’s inability to absorb or erase coherence constraints.

These correspondences demonstrate that SVET reproduces the classical conservation pillars not by postulating fields or symmetries, but by enforcing coherence consistency under a single, adjacency-preserving update rule.

---

## 5. Emergent Wave Mechanics
See Section 4.5 (Boundary Ledger and Tests) for the local ledger that determines surface reflection vs transmission.

### 5.1 Discrete Wave Equation

Wave-like behavior in SVET arises from repeated coherent updates across adjacency links in the node set. Each tick, a node exchanges directional flux with its neighbors according to local strain, bias, and cadence constraints. In the low-strain, low-latency regime, these local exchanges produce a discrete second-order update rule.

Let $\Phi(x,t)$ denote the coherent flux amplitude at node $x$ and tick $t$. The adjacency-based update rule takes the form:
$$\Phi(x,t+\Delta t) = 2\Phi(x,t) - \Phi(x,t-\Delta t) + c_{\text{eff}}^2 \sum_{x' \in \text{Adj}(x)} \left[\Phi(x',t) - \Phi(x,t)\right]$$

where:
- $\text{Adj}(x)$ is the set of nodes adjacent to $x$,
- $c_{\text{eff}}(x)$ is the effective propagation coefficient, which scales inversely with the local dilation factor $\alpha(x)$ and remaining budget $B(x) = 1 - U(x)$ (as established in Section 3.6):
  $$c_{\text{eff}}(x) = c_0 B(x) = c_0 \big(1 - U(x)\big)$$
  where $c_0$ is the baseline propagation speed in the unstrained vacuum.

In the long-wavelength limit, where variations across adjacent nodes are small, this discrete rule converges to the continuum wave equation:
$$\frac{\partial^2 \Phi}{\partial t^2} = c_{\text{eff}}^2 \nabla^2 \Phi$$

The effective propagation speed $c_{\text{eff}}$ is reduced relative to the invariant adjacency-hop limit $c$ whenever local strain or cadence penalties increase local utilization ($U \to 1$). This wave equation naturally incorporates medium-dependent propagation, dispersion, and cadence-induced refractive effects directly into the local capacity limits of the node set, recovering the asymptotic freezing of wave-packets near high-strain boundaries.

### 5.2 Interference via Flux Superposition

Interference in SVET arises from the superposition of coherent flux vectors arriving at a node with differing orientations and cadence delays. Because phase is encoded through directional alignment and timing (Section 2.4), interference requires no complex amplitudes.

Let two coherent contributions arrive at node $x$:
- flux vectors $\vec{F}_1$ and $\vec{F}_2$,
- cadence delays $\Delta t_1$ and $\Delta t_2$.

The combined coherent flux is:
$$\vec{F}_{\text{tot}} = \vec{F}_1 + \vec{F}_2$$
with the relative cadence delay producing an effective phase offset:
$$\Delta \phi = \omega (\Delta t_2 - \Delta t_1)$$
where $\omega$ is the local update frequency of the pattern.

Constructive interference occurs when the flux vectors align and cadence delays match:
$$\vec{F}_1 \parallel \vec{F}_2, \qquad \Delta \phi \approx 0$$

Destructive interference occurs when the flux vectors oppose or cadence delays differ by half a cycle:
$$\vec{F}_1 \approx -\vec{F}_2, \qquad \Delta \phi \approx \pi$$

Because flux is real-valued and directional, interference emerges from:
- vector addition of coherent update demand,
- cadence-induced timing offsets,
- and the local routing cost that modulates effective propagation speed.

This reproduces the full interference phenomenology of wave mechanics while remaining grounded in local, real-valued update rules.

### 5.3 Dispersion Relations
*TODO: Derive dispersion relations and define the effective refractive index \(n_{\text{SVET}}(\omega)\). Provide low‑frequency and high‑frequency asymptotics.*

---

## 6. Hilbert‑Space Correspondence

### 6.1 Amplitude as Coherent Flux Density

In SVET, amplitude is not a complex-valued field quantity but a real-valued measure of coherent flux density across the node set. For a pattern occupying a region $\Omega$ of nodes, the local amplitude $A(x)$ is defined as the magnitude of coherent flux arriving at node $x$ during a tick:

$$A(x) = \left\lVert F_{\text{coh}}(x) \right\rVert$$

This quantity reflects how strongly the pattern’s coherent structure is represented at that location. Because flux is capacity-limited (Sections 3.1–3.3), amplitude inherits strict upper bounds:

$$0 \le A(x) \le \min(B_x, u(\eta_x))$$

Amplitude in SVET therefore corresponds to the *locally realized coherent update density* rather than a continuous field amplitude. This mapping provides the bridge to Hilbert-space norms: higher coherent flux density corresponds to higher quantum amplitude in the continuum limit.

Amplitude is always ledger-tracked and pattern-level; it does not modify the underlying node-level update cadence or the invariant propagation limit $c$.

### 6.2 Phase from Orientation and Cadence

SVET encodes phase through two real-valued, locally defined quantities:

**1. Directional Orientation**  
The orientation of coherent flux across adjacency links determines the instantaneous phase direction of a pattern. Two patterns with identical amplitudes but differing flux orientations represent distinct phase states.

**2. Cadence Delay**  
Local variations in effective cadence $\tau_{\text{eff}}$ introduce timing offsets that act as discrete phase shifts. A delay of one tick corresponds to a fixed phase increment, and accumulated delays reproduce continuous phase evolution in the long-wavelength limit.

The effective phase at node $x$ is therefore:

$$\phi(x) = \phi_0 + \omega\,\Delta t(x)$$

where $\Delta t(x)$ is the accumulated cadence delay relative to a reference tick.

Because phase is encoded through orientation and timing rather than complex numbers, SVET reproduces interference, superposition, and phase evolution using only real-valued, locally computable quantities. This ensures that phase behavior remains grounded in the node set’s adjacency structure and cadence constraints.

### 6.3 Probability Density from Ledger Normalization

In SVET, probability density arises from the normalized distribution of coherent flux across the node set. Let $A(x)$ denote the coherent amplitude at node $x$ (Section 6.1). The total coherent amplitude of a pattern is:

$$A_{\text{tot}} = \sum_{x \in \Omega} A(x)$$

The probability density associated with node $x$ is then:

$$P(x) = \frac{A(x)}{A_{\text{tot}}}$$

This mapping reflects the fraction of the pattern’s coherent update demand realized at each node. Because amplitude is bounded and ledger-tracked, the normalization condition

$$\sum_x P(x) = 1$$

is automatically satisfied under the local ledger conservation algebra (Section 4.4).

Decoherence corresponds to the irreversible transfer of amplitude into the incoherent channel (Section 2.5). When coherent flux is shed into the $H$-channel, the corresponding probability weight is removed from the coherent distribution, reproducing the collapse-like behavior observed in measurement scenarios.

Thus, probability density in SVET is not an abstract postulate but a direct consequence of coherent flux distribution and ledger normalization.

### 6.4 Decoherence ↔ Heat Channel
*TODO: Formalize decoherence as irreversible transfer from coherent channel to heat channel and derive decoherence timescales.*

### 6.5 Eigenmodes and Pattern Persistence
*TODO: Define eigenmodes of the substrate and conditions for long‑lived patterns (quasi‑particles).*

---

## 7. QFT Correspondence Layer

The SVET framework reproduces the calculational structure of quantum field theory while replacing its continuum ontology with discrete, capacity-limited update rules. Fields, particles, propagators, and renormalization emerge as coarse-grained summaries of node-level dynamics rather than fundamental entities.

### 7.1 Fields as Statistical Summaries

Continuum fields arise in SVET as **statistical summaries** of node-level quantities over coarse-grained regions. For a region $\Omega$ containing many nodes, define the coarse-grained scalar, vector, or tensor field:

$$\Phi(x) = \frac{1}{\lvert\Omega\rvert} \sum_{i \in \Omega} q(i)$$

where $q(i)$ is the relevant node-level quantity (excitation, flux direction, strain component, etc.).

*   Scalar fields correspond to averaged excitation.
*   Vector fields correspond to averaged directional flux.
*   Tensor fields correspond to averaged strain.

Fields are not ontological primitives; they are **coarse-grained aggregates** of discrete update behavior. In the long-wavelength limit, these aggregates reproduce the continuum fields of QFT.

---

### 7.2 Excitations as Coherent Flux Packets

Particle-like excitations correspond to **localized, self-maintaining packets of coherent flux**. A coherent packet is defined by:

*   a stable flux orientation,
*   a bounded spatial support,
*   a cadence profile that maintains internal phase relationships.

The group velocity $v_g$ of a packet is determined by the **routing-cost gradient**:

$$v_g = \frac{\partial \omega}{\partial k}$$

where $\omega$ is the local cadence and $k$ is the effective spatial frequency.

Dispersion arises when different components of the packet experience different routing costs due to strain or excitation gradients. Stability requires that internal flux reinforcement exceeds incoherent shedding into the incoherent channel ($H$).

This reproduces the stability and propagation behavior of particle-like excitations in QFT.

---

### 7.3 Mass as Cadence Penalty

In SVET, inertial mass emerges from **cadence penalties** imposed by local excitation and routing cost. A pattern with higher internal excitation requires more update budget to maintain coherence, reducing its effective cadence:

$$\tau_{\text{eff}} = \tau_0 + \Delta \tau(\eta)$$

This cadence delay reduces the pattern’s ability to change its routing direction, producing inertial behavior.

*   Mass corresponds to resistance to cadence change.
*   Inertia corresponds to routing latency.
*   Relativistic mass increase corresponds to cadence slowdown under high excitation.
*   Relativistic momentum corresponds to **directional routing-cost accumulation**.

This mapping reproduces $E = mc^2$ as the cost of maintaining a coherent pattern.

---

### 7.4 Interactions as Local Strain Coupling

Interactions arise when overlapping coherent patterns modify each other’s **local strain field** and **update cost**. When two patterns overlap:

*   their strain fields superpose,
*   their routing costs shift,
*   their cadence profiles adjust,
*   their flux orientations redistribute.

The Node Rule resolves these competing demands by redistributing coherent flux, phase, momentum, and **orientation-like degrees of freedom**.

This redistribution is the SVET analogue of the interaction term in a Lagrangian. In the correspondence layer, **gauge interactions map to orientation-preserving flux constraints**, reflecting how certain flux orientations must be preserved under local update rules.

Thus:

*   QFT interactions $\leftrightarrow$ local strain coupling,
*   coupling constants $\leftrightarrow$ sensitivity of routing cost to strain,
*   gauge structure $\leftrightarrow$ orientation-preserving constraints in the correspondence layer.

---

### 7.5 Why Renormalization Disappears

Perturbation theory in QFT expands interactions into infinite series of virtual processes. In SVET, these “virtual particles” are not physical entities; they are **bookkeeping artifacts** of expanding the Node Rule into a series.

When patterns overlap, the adjacency structure must reconcile multiple update demands. The combinatorics of these reconciliations correspond exactly to the diagrammatic expansions of QFT.

Renormalization arises in continuum QFT because the underlying discrete update structure is replaced by integrals over unbounded momenta. SVET avoids these divergences because:

*   update capacity is finite,
*   excitation is bounded,
*   routing cost is finite,
*   cadence collapse prevents infinite frequencies,
*   the node-level update rule is discrete.

Thus, renormalization becomes **scale-dependent coarse-graining of update cost**, not a cure for infinities. The infinities of continuum QFT are replaced by finite, capacity-limited routing behavior in SVET.

---

## 8. GR Correspondence Layer

### 8.0 Discrete Time, Update Budget, and Relativistic Behavior

SVET models time as an ordered sequence of global ticks. At each tick, every node in the node set updates its state based solely on its own values and those of a finite set of adjacent neighbors. This discrete update structure replaces the continuum notion of time with a tick-indexed causal ordering.

Each node carries local quantities such as:
*   coherent flux amplitude,
*   phase,
*   orientation-like degrees of freedom,
*   local excitation,
*   local momentum-like routing bias.

Adjacency defines a finite propagation rate: exactly one hop per tick. This invariant hop rate corresponds to the causal ceiling identified with $c$.

In this framework, **energy corresponds to update demand**—the amount of local update work a pattern requires per tick. Patterns with higher excitation require more update budget to maintain coherence. When a pattern translates rapidly or must maintain coherence under strain, a larger fraction of the local update budget is spent on translation or coherence maintenance, leaving less available for internal cycles.

This produces:
*   **relativistic time dilation** as local pattern-level cadence slowdown,
*   **inertia** as resistance to changes in routing direction,
*   **rest energy** as the cost of maintaining internal coherence.

Tunneling arises naturally as **low-probability coherent leakage** across regions where the routing cost is high. In classically forbidden regions, the local update budget cannot support full propagation, but small-amplitude leakage persists due to the finite, discrete update rule. This reproduces quantum tunneling as a consequence of **capacity-limited update behavior**, not as a literal traversal of a potential barrier.

This discrete, capacity-limited update picture forms the foundation for the GR correspondence layer. Spatial gradients in the effective cadence field $\tau_{\text{eff}}(x)$ produce the macroscopic phenomena interpreted as curvature, geodesic motion, and horizon formation.

*For gravitational redshift and time dilation, see Section 15.1 (Unified Redshift Theory), which provides the full exaction-potential derivation [1].*

### 8.1 Curvature as Cadence Gradient

In SVET, gravitational curvature is not a geometric property of a manifold, but an emergent Layer 2 observation of the Layer 1 Resolution Latency Gradient. The Background Exaction Bias ($\Psi$) at any adjacency-indexed region is the cumulative ledger-resolved exaction bias resolved by the local nodes. Due to Node-Set Blindness, the hardware does not distinguish between pattern-specific exactions and the cumulative background load; it simply executes the update rules against the available Tick-Budget ($B$). A perfectly uniform $\Psi$ across an adjacency-indexed region is ledger-neutral regarding pattern routing. While a uniform bias increases the total exaction load, it does not create a directional update bias. In this state, the Resolution Latency ($\tau_{eff}$) is increased uniformly, but no gradient exists to deflect the Instantiation Trajectory of a pattern. When the background exaction bias is non-uniform ($\nabla \Psi \neq 0$), it creates a Cadence-Suppression Gradient. Because the Tick-Budget ($B$) is a finite local parameter, nodes in adjacency-indexed regions of higher $\Psi$ experience higher Utilization ($U$). This results in a localized increase in the number of node-set update intervals required to resolve a single pattern-level update:

$$ \tau_{eff}(x) = \tau_0 \cdot f(U(x)) $$

where $\tau_0$ is the invariant hardware interval defined by Tick Invariance. A pattern traversing this gradient must resolve its internal instruction set across nodes with varying resolution latencies. The resulting deflection of the Instantiation Trajectory toward regions of lower exaction cost (lower $U$) is what the macroscopic observer models as "gravitational curvature." Gravity is therefore not a force, but the gradient response of the node-set utilization profile.

### 8.2 Geodesics as Least‑Delay Paths
The equivalence principle is naturally recovered as a local kinematic property of the node network. In SVET, gravitational acceleration is not a force, but the result of a spatial gradient of cadence ($\nabla \tau_{\text{eff}}$). A propagating wave pattern in free fall simply rides this local cadence tilt. Because the pattern's internal update cycles are uniformly adapted to the local latency, this gradient remains locally undetectable to the pattern itself—the tilt is locally invisible. Measurable physical effects only manifest as tidal strain gradients, where non-uniform variations in the cadence gradient across an extended pattern create differential update latencies that cannot be locally adapted out.

### 8.21 Excitation Propagation, Motion, and the Meaning of Gravity

In SVET, patterns propagate through local updates across adjacency links. Interactions arise from local reconfigurations of coherent flux, not from point‑particle translation. Motion is therefore not the displacement of a material object but the redistribution of coherent flux across nodes.

Translation consumes update budget. A pattern that moves must allocate part of its finite update capacity to maintaining directional coherence. This creates a local bias in the update rule — a coherence‑strain — that influences how subsequent updates propagate. Patterns follow paths that minimize accumulated update cost. These coherence‑minimal paths are the SVET analogue of geodesics.

Mass and energy correspond to baseline and dynamic update demand. The rest‑frame update cost is the budget required to maintain a coherent pattern when not translating. Additional strain increases the local cadence penalty, slowing internal cycles and producing relativistic time dilation.

Changes in exaction distribution modify the local cadence field. These modifications propagate outward at the invariant hop rate c, appearing macroscopically as gravitational influence. In the continuum limit, these propagating cadence‑bias adjustments reproduce the tidal phenomena attributed to curvature in General Relativity.

Under this interpretation, gravity is not a force and not a geometric property of a manifold. It is the macroscopic expression of how coherence‑constraint sets are resolved under finite update budgets in a discrete, capacity‑limited system. Horizons correspond to limits of pattern coherence, not literal infinities in spacetime geometry.

### 8.22 Scale-Dependent Cadence Gradient Response

The apparent weakness of gravity at the quantum scale is a topological consequence of the ratio between the adjacency-indexed region size ($L$) of a pattern and the local exaction-bias gradient ($\nabla \Psi$). Because a pattern resolves its internal instruction set through the differential in resolution latency ($\Delta \tau_{eff}$) across its constituent node-set update intervals, its sensitivity to curvature is strictly scale-dependent.

For a quantum-scale pattern where $L$ is small, the background exaction bias ($\Psi$) is effectively uniform across the pattern's adjacency-indexed region. In this regime, the differential $\Delta \tau_{eff} \approx 0$, and the pattern executes as if the local exaction floor were flat. This defines the **Local Uniformity Threshold**: the scale at which the cadence-suppression gradient magnitude is below the resolution threshold of the pattern's internal update dynamics. In this state, the pattern’s internal dynamics are dominated by its own high-frequency exaction profile, rendering the gentle tilt of the background bias dynamically negligible.

Conversely, for macroscopic patterns where $L$ spans a significant gradient of $\Psi$, the differential $\Delta \tau_{eff}$ across the adjacency-indexed region becomes dominant. The influence of curvature is characterized by the ratio $R_{SVET} \approx (|\nabla \Psi| \cdot L) / \Psi_{int}$, where $\Psi_{int}$ represents the pattern's internal exaction intensity. As $L$ increases, $R_{SVET}$ rises, leading to the observable deflection of the instantiation trajectory. The transition from the quantum regime to the macroscopic regime is therefore a continuous scaling of the ratio between pattern size and the local exaction-bias gradient, rather than a shift in underlying physical laws.

### 8.3 Horizons as Capacity Boundaries
*TODO: Define horizons as surfaces where \(\tau_{\text{eff}} \to \infty\) or where coherent propagation is effectively halted.*

### 8.4 Finite‑Core Black Holes and Horizon Formation

In SVET, black holes arise when extended regions exceed the collapse excitation threshold $\eta_{\text{BH}}(R)$. Unlike General Relativity, the interior of a collapsed region is not forced into a coordinate or physical singularity. Instead, the node set experiences **Cadence Collapse**, asymptotically approaching its finite excitation ceiling without reaching literal zero-tick.

#### The Asymptotically Frozen Interior
As the excitation approaches saturation ($\eta \to 1$) within the interior, the effective cadence diverges asymptotically: each incremental increase in $\eta$ produces exponentially larger slowdowns in $\tau_{\text{eff}}$, analogous to how approaching the speed of light requires exponentially increasing energy. In the weak-field limit, cadence collapse reproduces gravitational redshift and time dilation, with the effective cadence $\tau_{\text{eff}}$ serving as the SVET analogue of the GR lapse function $g_{00}$, not as a dynamical metric component but as a pattern-level cadence field emerging from excitation.

The underlying node set continues to propagate update states at the absolute, structural propagation limit $c$ (one adjacency hop per tick) to maintain the local transmission of strain fields. What collapses is the ability of the extended, coherent pattern to exploit that raw network capacity. The interior never reaches a state of literal zero-tick or total cessation of updates; rather, it approaches this frozen state asymptotically. Because the local excitation cannot exceed the absolute microphysical ceiling ($\eta_{\max} = 1$), the interior is preserved as a finite, non-singular, and stable domain of highly latent state updates.

#### Coherence Horizon
A horizon forms where outward coherence routing becomes impossible because the local update costs exceed any possible local coherence budget:
$$\eta(r) \to \eta_{\text{BH}} \quad \Rightarrow \quad \text{coherence horizon}$$
The collapse threshold $\eta_{\text{BH}}(R)$ marks the point where strain-induced bias forces the coherence cost $C(x,v)$ to diverge, driving $\tau_{\text{eff}} \to \infty$ and forming a coherence horizon. This boundary is a localized routing limit, not a geometric or spatial tear in the network. Because the horizon blocks pattern-level propagation while allowing background node bookkeeping to continue normally, gravity waves and strain information propagate past the boundary without violating causality. Macroscopically, this collapse threshold recovers the classical general relativistic Schwarzschild boundary condition:
$$R \le R_s = \frac{2GM}{c^2}$$

#### Universality Across Scales
The identical physical mechanism governs stellar-mass black holes, supermassive black holes, and micro-black holes formed by Planck-scale probes. All share the same fundamental features: a finite, saturated interior governed by asymptotic cadence collapse, and a coherence horizon defined by the limit of the local update budget.

### 8.5 Hill vs. Hole Duality

To establish the general relativistic correspondence layer, we must clarify the fundamental physical contrast between the continuous geometric potential well of General Relativity and the discrete, exaction-spending update ledger of SVET. 

#### 1. The Conceptual Contrast
*   **General Relativity (The Potential Hole):** Classical physics models gravity as a negative potential well, a geometric "hole" warped into a continuous spacetime manifold. Spacetime itself acts as an active, deformable background that is bent by the presence of mass, pulling trajectories inward [1].
*   **SVET (The Exaction Hill):** In contrast, SVET models gravity as a positive exaction-strain hill resting on a completely flat, static, and non-deforming node set. The node set does not warp, bend, or pull; it simply exists as static adjacency and available budget. A high-exaction-density exactor pattern does not "dig a hole" in space; rather, its highly complex exactions compel the local node set to spend its update budget, causing local utilization ($U = S/B$) to inflate [1]. 

This localized budget expenditure manifests as a positive "utilization hill." Time dilation is not a descent into a geometric well, but an ascent onto a highly utilized exaction-strain hill, where the pattern's effective cadence slows because the local nodes are heavily burdened by background spending.

#### 2. The Weak-Field Shadow (Local Equivalence)
Despite operating on opposite physical mechanisms, one geometric and negative, the other dynamical and positive, the two theories cast the identical mathematical shadow in the weak-field limit [1].

In General Relativity, the coordinate time interval $dt$ required to resolve a local proper time step $d\tau$ at radius $r$ in a weak gravitational potential $\Phi = -\frac{GM}{r}$ is expressed via the inverse square root:
$$dt = \frac{d\tau}{\sqrt{1 - \frac{2GM}{r c^2}}} \approx d\tau \left(1 + \frac{GM}{r c^2}\right)$$

In SVET, the local coordinate update interval $dt(r)$ required to complete a pattern-level exaction-resolution step scales with the local update latency (the cadence slowdown) driven by local utilization $U(r)$ [1]:
$$dt(r) = \tau_0 \alpha(r) = \tau_0 \left(\frac{1}{1 - U(r)}\right)$$
Evaluating this coordinate update interval relative to a distant, un-strained reference tick ($dt_0 = \tau_0$) in the weak-field limit yields the positive series expansion:
$$dt(r) = dt_0 \left(\frac{1}{1 - U(r)}\right) \approx dt_0 \big(1 + U(r)\big)$$

Under the weak-field correspondence mapping:
$$U(r) \;\leftrightarrow\; \frac{GM}{r c^2}$$
these two coordinate time interval equations collapse onto the identical positive-sign coordinate dilation shadow [1]. The local cadence-suppression gradient ($\nabla \tau_{\text{eff}}$) of the static node set perfectly reproduces the gravitational redshift and lensing behaviors predicted by General Relativity's metric tensor.

#### 3. Strong-Field Divergence (Singularity Avoidance)
While the two theories match far out in the weak-field regime, they diverge cleanly in the strong-field limit near $U(r) \to 1$ [1]. 

In General Relativity, because the math has no self-limiting structural ceiling, the negative well continues down to an infinite coordinate singularity at the center ($R \to 0$), resulting in infinite curvature and a breakdown of physical laws.

In SVET, the local exaction-utilization hill is bounded asymptotically by the Planck Saturation Ceiling ($U \le 1$). Through the mechanism of Asymptotic Cadence Collapse, each step toward saturation ($U \to 1$) requires exponentially higher local exaction densities, producing exponentially larger slowdowns in the effective cadence ($\tau_{\text{eff}} \to \infty$) without ever reaching a literal halt in parameter evolution [1]. The interior never reaches a true cessation of parameter updates; rather, it approaches this non-singular, stable state asymptotically, completely eliminating the mathematical singularities of General Relativity [1].

### 8.6 Relativistic Stability Limits and Tidal Fracture
While gravity is geometrically described by spatial gradients of the cadence field ($\nabla \tau_{\text{eff}}$), the physical entities propagating through these fields are finite, extended coherence-patterns. Under extreme conditions, these patterns experience structural degradation:

*   **Time Dilation ($\Delta \tau$):** As a pattern enters a high-strain region, its internal update processes slow down. The resolution latency ($\Delta \tau$) required to complete a single internal update cycle increases relative to distant, unstrained nodes.
*   **Stability under Strain ($\Gamma_p$):** A pattern can only maintain its structural coherence if the local strain-to-budget ratio ($S/B$) remains below its intrinsic stability threshold ($\Gamma_p$). If this threshold is crossed, the pattern reaches its physical limit and undergoes structural yield, fracturing into incoherent energy within the $H$-channel.
*   **Tidal Gradient Response:** In regions with steep cadence gradients ($\nabla \tau_{\text{eff}}$)—such as near a high-excitation core—different parts of an extended coherence-pattern experience uneven latency. The leading edge of the pattern updates at a different rate than the trailing edge, stretching its internal node bindings. This spatial discrepancy destabilizes the pattern's structural integrity, triggering a localized $\Gamma_p$ collapse into simpler, incoherent excitations.

*TODO: Describe the structural incompatibility between a pattern’s internal wave-geometry and the propagation geometry demanded as its effective velocity approaches the adjacency-hop limit ($c$). Explain how this geometric mismatch increases $\Delta\tau$, elevates strain, and drives the pattern toward $\Gamma_p$-limited collapse.*

### 8.7 Coherence Manifold GR Correspondence

When the directional cost function $C(x,v)$ admits a quadratic velocity form, the effective metric $g_{\mu\nu}(x)$ governs macroscopic propagation. Under this mapping, spatial update preferences define the geometry:
*   **Radial Update Bias:** High radial strain biases the node network toward inward updates, producing the emergent metric effect of gravitational attraction.
*   **Tangential Update Bias:** High tangential strain biases the network toward sideways updates, producing the macroscopic equivalent of frame-dragging.
*   **Boundary Horizons:** Critical cost boundaries arise where outward propagation costs exceed any possible local coherence budget ($B \to 0$), creating one-way routing surfaces where outward geodesics terminate.

### TODO: Black Hole Correspondence Integration (See `SVET_issues_list.xls` — Tab “SVET Blackhole”)

A full integration of SVET’s black hole modeling framework is postponed pending completion of the GR and QFT correspondence layers. The following items have been reviewed and triaged for structured incorporation:

* Horizon formation as a coherence-budget limit  
* Ergosphere as mandatory azimuthal-update region  
* Spin and charge as distinct strain channels  
* Redshift as cadence mapping and coherence-throughput reweighting  
* Cold-interior interpretation (local vs. asymptotic update rates)  
* Toy budget equation: $B(r) = C_{\text{max}}(r) - (S_r^2 + S_{\theta}^2 + S_Q^2)$  
* Inspiral frequency ceiling and ringdown deltas  
* Interior pattern-class reconstruction from exterior observables  

These items are tracked in `SVET_issues_list.xls`, Tab **“SVET Blackhole”**, and will be integrated once the correspondence scaffolding is finalized.

---

## 9. Causal Boundaries

### 9.1 Maximum Update Rate
*TODO: Define the substrate's maximum update rate and its role in setting a maximum signal speed.*

### 9.2 Adjacency‑Limited Propagation
*TODO: Formalize adjacency hop limits and their effect on causal structure.*

### 9.3 Emergent Lorentz Symmetry
*TODO: Provide arguments and calculations showing how Lorentz symmetry emerges in the long‑wavelength limit from cadence and adjacency constraints.*

### 9.4 The Double-Walled Universe: Cosmic and Quantum Boundaries

The SVET framework unifies the microscopic and macroscopic limits of the cosmos, showing that the physical universe is bounded by two symmetric, non-singular causal walls. Both boundaries are emergent manifestations of the identical physical phenomenon: asymptotic **Cadence Collapse** at opposite ends of the scale axis.

#### 1. The Quantum Wall (Small-Scale Boundary)
At the microscopic limit, attempting to probe scales smaller than the Planck length requires concentrating high-energy density into an increasingly localized region. When a Planck-scale probe focuses energy into a volume smaller than its local coherence horizon, the local excitation is driven toward saturation ($\eta \to 1$). 

Through the mechanism of cadence collapse, the local update delays diverge asymptotically. The resulting frozen state prevents further coordinate probing or deeper information extraction, establishing an absolute, non-singular lower boundary on physical measurements. Throughout this transition, the underlying nodes continue to tick normally at the hardware limit $c$; only the pattern-level resolution latency diverges. At the quantum wall, the local excitation approaches the collapse threshold $\eta_{\text{BH}}(R)$, forcing the coherence cost $C(x,v)$ to diverge and driving $\tau_{\text{eff}}$ toward its asymptotic limit.

#### 2. The Cosmic Wall (Large-Scale Boundary)
At the macroscopic limit, the cosmological expansion of the universe outruns the maximum coherent update propagation rate ($c = 1$ node per tick). At this boundary, the effective local cadence of the distant node set slows asymptotically relative to a local observer, triggering a cosmic-scale cadence collapse that forms the Hubble coherence horizon. 

Beyond this boundary, the budget required for coherent propagation diverges, preventing further coherent information from reaching the observer.

#### Ontological Unification
These two boundaries—the Planck-scale quantum wall and the Hubble-scale cosmic wall—are symmetric limits of the same underlying capacity constraint. At both scales, the network's update budget undergoes asymptotic cadence collapse, establishing a finite, non-singular "soft box" within which all physical patterns must propagate.

Furthermore, this unified boundary structure encodes how local gravitational strain suppresses the cosmological Hubble flow. At small scales, the localized update demands of matter dominate, completely suppressing the global expansion rate. The universal horizon variable $U$ must therefore capture this competitive scaling transition, mapping how the node set transitions from locally gravity-dominated to cosmologically expansion-dominated regimes.

Because both the Quantum Wall and the Cosmic Wall arise when exaction approaches its collapse threshold and the effective cadence diverges, the candidate universal horizon variable $U$ must be a monotonic function of $\eta$ and $\tau_{\text{eff}}$, saturating near the quantum wall ($U \to 1$) and vanishing near the cosmic wall ($U \to 0$). This constraint ensures that $U$ serves as the primary candidate axis along which GR-like, SVET-like, and QG-like regimes align, enabling mass-independent curve collapse and forming the mathematical backbone of the Universality Scoring System [1].

---

## 10. Measurement and Decoherence
*TODO: Clarify the observational criterion for pattern integrity: a pattern remains operationally intact as long as an observer can receive coherent signals from it. Define the boundary between detectable coherence, partial decoherence, and full collapse into the incoherent channel (H).*

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

### 11.6 Localized Exaction Overload: Plasticity as Low-Energy Arithmetic Collapse

In SVET, material deformation is not governed by continuous physical forces or field-mediated potentials. Instead, both low-energy mechanical deformation (plasticity) and high-energy state reconfigurations (particle showers) are unified under a single, discrete mechanism: the local update rules resolving exaction demands against a finite available budget.

#### 11.6.1 Elastic Regime (Coherent Constraint Preservation)
In the elastic regime, the local strain $S(x)$ increases while the coherence-constraint set of the pattern remains entirely intact. The local available budget is sufficient to satisfy the local and adjacency exaction demands without requiring any modifications to the pattern's configuration. When the external exaction load is removed, the pattern reconstructs its original configuration because no permanent coherence-constraint reconfiguration has occurred.

#### 11.6.2 The Arithmetic Collapse Threshold (The Yield Point)
As local strain $S(x)$ approaches the node-set-level yield threshold $\kappa_{\text{yield}}$, the node set can no longer satisfy the requested adjacency-coherent continuation within the available tick-budget $B$. Any attempted exaction exceeding this limit is immediately clamped, with the unresolvable excess diverted into the incoherent channel as a coherence-shedding increment $\Delta H$ to maintain local ledger closure. This local arithmetic subtraction marks the yield point.

#### 11.6.3 Plastic Regime (Constraint-Set Reconfiguration)
Plastic deformation is the permanent, step-by-step reconfiguration of a material's coherence-constraint set following a local coherence-shedding event. Once local strain $S(x)$ reaches the yield threshold $\kappa_{\text{yield}}$, the local update rules resolve the exaction conflict by permanently altering the local adjacency-coherent structure. The resulting $\Delta H$ output dissipates, but the updated constraint topology persists and becomes the new target for all subsequent node-tick reconstructions. This mechanism is the SVET analogue of dislocation motion, slip, and permanent set in classical materials science, occurring without any background metric or field-theory dynamics.

#### 11.6.4 Residual Strain, Material Memory, and Work Hardening
Because the coherence-constraint set is permanently altered, the material retains a physical memory of the high-strain event. This memory is encoded directly in the updated constraint topology, not in the incoherent $H$-channel. 

Crucially, this reconfigured topology expands its effective adjacency footprint, distributing future exaction loads across a larger local neighborhood. This reduces local strain density during subsequent deformation attempts, naturally increasing the effective stability margin and producing the macroscopic signature of work hardening.

#### 11.6.5 Stability Margin ($\Gamma_p$) as a Derived Diagnostic
Although not an ontological primitive of the node set, the stability margin $\Gamma_p$ serves as a practical, derived diagnostic for materials-science applications. It provides a post-facto scalar summary of how close the local strain $S(x)$ is to the invariant, node-set-level yield threshold $\kappa_{\text{yield}}$:
$$\Gamma_p(x) \equiv 1 - \frac{S(x)}{\kappa_{\text{yield}}}$$
$\Gamma_p(x)$ is strictly clamped to the interval $[0,1]$, where $\Gamma_p = 0$ marks the yield threshold. At extreme strain levels, we observe:
$$U(x) \to 1 \quad \Rightarrow \quad \Gamma_p(x) \to 0$$
This parameter carries no physical agency and does not modify local update resolution; it is a convenience metric summarizing the remaining stability margin of a coherence-constraint set under strain [1]. All dissipation remains the instantaneous, arithmetic remainder of an overloaded exaction event, with variations in $\Gamma_p(x)$ serving as a diagnostics tool to track the cumulative evolution of constraint-set configurations [1].

### 11.7 Casimir Effects and Vacuum Exaction Constraints

SVET reinterprets the Casimir effect not as the result of geometric boundary conditions on a continuous field, but as the suppression of vacuum exaction-patterns by the quantization limits of the node set [1].

#### 11.7.1 The SVET Casimir Correction Ansatz
The classical Casimir force between two ideal, perfectly conducting plates in vacuum separated by distance $a$ is defined as:
$$F_0 = -\frac{\pi^2 \hbar c}{240 a^4}$$

SVET predicts a discrete correction term $\delta$ that emerges as the plate separation approaches the functional granularity of the node set. The corrected force is expressed as:
$$F_{\text{SVET}} = F_0 \big[1 + \delta(a; \ell_{\text{node}}, \Delta t, R_{\text{mat}})\big]$$

These corrections arise because SVET enforces quantization limits on vacuum modes through node-spacing granularity, tick-duration temporal resolution, and update-budget capacity ceilings [1, 2]. Vacuum modes that cannot be instantiated within these limits are suppressed outright, producing discrete deviations from the continuum Casimir force [1, 2]. As $a/\ell_{\text{node}} \to \infty$ (the continuum limit), the correction $\delta \to 0$, recovering the standard macroscopic result.

#### 11.7.2 Material Density and Depth of Constraint
Unlike standard Lifshitz theory, which relies on macroscopic dielectric functions $\epsilon(\omega)$, SVET provides additional degrees of freedom based on the local node-set architecture of the plates:

*   **Exaction-Density Suppression:** Denser or more rigid coherence-constraint sets in the plate nodes impose a stronger suppression on vacuum patterns, increasing the magnitude of the Casimir effect.
*   **Internal Coherence-Constraint Modes:** If the plate nodes possess specific internal coherence-constraint modes, they can interact constructively or destructively with specific vacuum exaction-profiles in ways not captured by a smooth dielectric function [1].
*   **Thickness as Constraint Depth:** SVET predicts that the total thickness of a plate influences the vacuum exaction budget even beyond the classical EM skin depth. A thinner, highly rigid configuration may exert a different constraint than a thicker, loosely constrained configuration, even if their macroscopic refractive indices are identical.

#### 11.7.3 Thermal Coherence Load and Casimir Scaling
In SVET, the temperature of the plates and the surrounding environment is defined as the average Thermal Coherence Load (pattern-internal exaction density) [1]. 

*   **Cryogenic Regime:** Plate and vacuum nodes are at minimal thermal exaction load ($\eta \to \eta_{\text{vac}}$), allowing the node set to resolve vacuum exactions with maximum precision.
*   **Thermal Regime:** Nodes are burdened by non-directional patterns. This Thermal Coherence Load populates additional update modes, reproducing the standard thermal Casimir scaling in the continuum limit [1].

The SVET-native version of the thermal exaction-density differential is:
$$\Delta \rho(a; T) = \int [g_{\text{plates}}(\omega, a; T) - g_{\text{free}}(\omega; T)] \, \epsilon(\omega, T) \, d\omega$$
where $g$ represents the allowed pattern density and $\epsilon(\omega, T)$ is the exaction demand per mode, including the thermal component of the exaction budget [1].

#### 11.7.4 Extreme Regime Deviations and Falsifiability
SVET predicts systematic deviations from standard Lifshitz-Casimir predictions at extreme temperature limits:

1. **Low-Temperature Freeze-Out:** At cryogenic limits, the internal exactions of the plate nodes may rigidify in a way that alters how they suppress specific vacuum modes, producing a non-linear deviation from standard low-T predictions [1].
2. **High-Temperature Saturation:** At extreme temperatures, as plate nodes approach the Planck Saturation Ceiling ($U \to 1$), their available local update budget for resolving vacuum exactions is exhausted. This predicts a saturation or "cutoff" of the Casimir force that standard EM does not model [1].

These effects are expressed through a temperature-dependent correction $\delta_T$, which is not derivable from the macroscopic dielectric function $\epsilon(\omega, T)$ alone, providing a clear pathway for experimental falsification [1].

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

### TODO: Archive and Integrate Early Toy Model Documentation (See `SVET_issues_list.xls` — Tab “SVET Onboarding v0.02–0.03”)

The early SVET onboarding narrative (v0.02–v0.03) has been reviewed and triaged. Its content describes the initial lattice toy model, diagnostics, CSV logging, and the three redshift experiments. These items are engineering artifacts and will be incorporated into the Appendix as historical context once the computational layer is finalized.

---

## 13. Predictions and Falsifiable Tests
Possible 13.6 Reflectivity, Decoherence, Plastic deformation. Experimental slab test described in Section 4.5 provides a direct falsifiable test of SVET partitioning.
**Experimental dependencies:** The predictions below assume the pattern‑dependent yield formalism of Sec. 2.6 Incoherent Channel (H) and the node partition identity of Sec. 4.4 The Node Ledger. Simulation protocols in Sec. 11 Computational Implementation Layer provide the reproducible logging required to compare measured R, T, and H against SVET predictions.

### 13.1 Pump‑Induced Refractive Index Shifts
*TODO: Quantify predicted index shifts under intense pumping and propose pump‑probe experimental setups.*

### 13.12 Coherence Manifold Predictions

*   **Horizon Boundary Routing:** Horizon surfaces are predicted to block coherent pattern propagation due to budget exhaustion ($B \to 0$) while allowing background node bookkeeping to continue normally, preserving local causality and preventing any coordinate or physical singularities.
*   **Asymmetric Wavefront Arrival:** Tangential update bias regions (ergospheres) are predicted to produce measurable, direction-dependent propagation time delays in coherent wave packets.
*   **Inspiral Frequency Saturation:** Binary inspiral frequencies are predicted to reach a hard ceiling where localized utilization $U(r)$ forces a routing collapse, providing a signature in high-precision wave spectra.

### 13.2 Finite‑Core Black Hole Signatures
*TODO: List observational signatures (e.g., modified ringdown, core emission spectra) that distinguish finite‑core black holes from classical singularities.*

### 13.3 Cadence‑Based Lensing Deviations
*TODO: Predict small deviations from GR lensing due to cadence gradients and propose observational tests.*

### 13.4 SVET‑Specific Dispersion Curves
*TODO: Provide dispersion curves for SVET and compare to standard QFT/GR expectations.*

### 13.5 Decoherence‑Rate Predictions
*TODO: Provide quantitative decoherence rates for mesoscopic systems and suggest laboratory tests.*

### 13.6 The Yield Ramp Test
*Simulation:* Locally increase update demand ($S_p$) at a node ensemble and measure the critical $S/B$ ratio where coherent amplitude collapses into the H-channel.
*Target:* This test uses a reference pattern with $\Gamma_p = 1$ under slow loading to isolate the universal constant $\kappa_{\text{yield}}$.

### 13.7 Loop Integrity and Confinement
*Simulation:* Model a coherent loop (particle) under increasing external strain. 
*Target:* Verify if a loop yield event produces energy-conserving pair excitations. For high $\Gamma_p$ patterns, yield events are irreversible, providing a node-network explanation for quark confinement.

### 13.8 Measurement Statistics (Born Rule Emergence)
*Simulation:* Model a detector as a localized strain source. 
*Target:* Demonstrate that "Wavefunction Collapse" statistics emerge from the yield event of the wave pattern, converging to Born-rule frequencies over repeated trials.

### 13.9 Coherence Recovery Test
*Simulation:* After a near-yield ramp, reduce $S_p$ and observe whether the pattern re-establishes coherence. 
*Target:* Robust patterns (high $\Gamma_p$) should recover; fragile patterns may not. Record hysteresis and recovery times to distinguish reversible vs. irreversible yield.

### 13.10 Nuclear Resonance Windows as SVET Coherence Modes
This predictive test maps standard nuclear stability and decay profiles to the discrete geometric resonance modes of the node network. Rather than relying on independent field-mediated interactions, we re-interpret nuclear configurations as localized, high-density coherence-patterns:

*   **Coulomb Repulsion:** Modeled as localized coherence-strain ($S$) arising from overlapping update demands.
*   **Strong Interaction:** Modeled as "coherence locking," where adjacent nodes coordinate their phase states to minimize overall update cost.
*   **Nuclear Shell Model:** Modeled as discrete, allowed spatial resonance modes that fit the local node horizon geometry.
*   **Instability & Decay (Coherence Catastrophe):** Heavy nuclei undergo structural yield and fall apart when the total coherence-strain ($S$) required to sustain their internal wave-geometry exceeds the available local budget ($B$) of the node network.

**Experimental Target:** Map the specific mass numbers of known islands of stability and correlate them with localized node-network resonance windows, predicting decay rates based on the available local budget-to-strain ratios.

### 13.11 QED-Regime Budget Tests

Once the budget equation is defined explicitly, SVET predictions can be mapped to laboratory observables. The governing relation is:

$$B(r) = \frac{1}{1 + \eta(r)} \quad \text{or more generally} \quad B(r) = \frac{1}{1 + f(\eta(r))}$$

Here, $\eta(r)$ represents local strain-to-demand ratio, and $B(r) \to 0$ marks the onset of coherence collapse. This limit corresponds to the Schwinger threshold expressed in SVET language.

**Observable consequences of budget exhaustion:**

*   **Pair production rate** — $B \to 0$ $\to$ vacuum breakdown $\to$ measurable electron-positron pairs.  
*   **High-order harmonic cutoff** — budget depletion $\to$ nonlinear refractive index $\to$ spectral shifts.  
*   **Vacuum birefringence** — anisotropic strain $\to$ polarization rotation.  
*   **Pulse steepening / self-compression** — budget bottleneck $\to$ effective dispersion $\to$ measurable in plasma-mirror experiments.

These effects provide direct experimental handles for testing SVET’s coherence-budget formalism against strong-field QED data.

### TODO: Supporting Artifacts for QED-Regime Budget Tests (See `SVET_issues_list.xls` — Tab “SVET QED Maths”)

The following supporting materials will be generated after correspondence calibration:

*   **Lab-Test Checklist** — defines measurable observables and experimental setups for validating SVET’s budget-collapse predictions.  
*   **Budget-Sweep Simulation Pseudocode** — outlines parameter sweeps for $B(r)$ across strain and cadence gradients.  
*   **QED-Math Triage Summary** — consolidates mappings between SVET variables and standard QED quantities for cross-comparison.

These placeholders ensure that the QED-testability framework remains visible and will be revisited once the correspondence layer and experimental calibration are complete.

### 13.13 Classical Pathology Resolution Tests

#### 13.13.1 Painlevé-Type Constraint Failure Resolution (SVET Prediction)

Classical rigid-body mechanics exhibits the Painlevé paradox: certain contact-interaction configurations admit no consistent solution under Newtonian constraints, producing non-existence, non-uniqueness, or formally infinite accelerations. These pathologies arise from the classical assumption of instantaneous constraint enforcement and unbounded reaction forces.

SVET predicts that Painlevé-type inconsistencies cannot occur in any physical system. Because all pattern-level interactions are resolved through finite tick-budget, finite strain $S(x)$, and cadence-limited reconstruction, no pattern can impose an instantaneous or infinite constraint. When a classical Painlevé configuration would require an inconsistent or unbounded reaction force, the local update rules resolve the conflict through Accounting Shock (coherent rejection) and $\Delta H$ shedding (incoherent remainder). The coherence-constraint set reconfigures rather than enforcing an impossible constraint.

**Prediction:**  
Any experimental system engineered to reproduce a Painlevé-type inconsistency will instead exhibit finite, cadence-limited reconstruction delay, coherence-shedding ($\Delta H$), or constraint-set reconfiguration, never infinite acceleration or non-existence of solutions.

**Falsifiability:**  
If a physical system can be shown to produce a true Painlevé non-solution or infinite acceleration without material compliance, SVET is falsified.

#### 13.13.2 Catalog of Classical Pathology Resolutions

Because the vacuum does not consist of a continuous coordinate manifold, no continuous physical forces exist. In SVET, all classical mechanical pathologies and non-integrable constraints are resolved through local, discrete, and capacity-limited exaction bookkeeping. Below is the compiled catalog of classical paradoxes resolved natively under this single-equation update engine:

**1. Zeno’s Paradoxes (All Variants)**  
*   **Classical Failure:** Infinite subdivisions of space and time imply that motion is mathematically impossible.  
*   **SVET Resolution:** The universe is built from a discrete node set; there is no continuous coordinate space and no infinite subdivisions. Motion is not continuous translation; it is the discrete, tick-indexed instantiation of adjacency-hop exactions across neighboring nodes. Under the Single-Tick Identity Principle (STIP), identity is frozen, and motion is reconstructed strictly as the sequence of differences between ticks.  
*   **Mechanism:** STIP + adjacency-hop exactions + $\Delta\tau$ latency.

**2. D’Alembert’s Paradox (Zero Drag in Ideal Fluids)**  
*   **Classical Failure:** The Euler equations of fluid dynamics predict that a body moving through an incompressible, inviscid fluid experiences zero drag.  
*   **SVET Resolution:** An ideal, lossless continuum does not exist. Every moving pattern undergoes a directional coherence-shedding tax ($\Delta H$) as its exactions are propagated. Fluid flow patterns impose local coherence-shearing across the node set, forcing a portion of the exactions to collapse into incoherent $H$-channel deviations.  
*   **Mechanism:** $\Delta H$ shedding + Coherence-Constraint Reconfiguration.

**3. Painlevé Paradox (Rigid-Body Contact with Friction)**  
*   **Classical Failure:** Certain friction coefficient and contact angle combinations produce non-existence or infinite accelerations under classical Newtonian constraints.  
*   **SVET Resolution:** Friction is not an active force; it is the directional coherence cost density $C(x,v)$ of propagating a pattern across a strained node set. Impossible constraints simply drive the local resolution latency $\Delta\tau$ toward its asymptotic limit, and the local ledger resolves the exaction conflict via Accounting Shock (coherent rejection) and $\Delta H$ shedding.  
*   **Mechanism:** $\Delta\tau$ latency + $C(x,v)$ cost + Accounting Shock.

**4. Rigid-Body Impact Paradox (Infinite Impulse)**  
*   **Classical Failure:** Colliding rigid bodies require an infinite impulse to reverse velocity instantaneously in zero time.  
*   **SVET Resolution:** There are no perfectly rigid bodies, and no instantaneous constraint enforcement is permitted. An impact is resolved as a finite sequence of $\Delta\tau$-delayed instantiations; any excess exaction demand that cannot be accommodated within the local tick-budget $B$ is safely shed as $\Delta H$.  
*   **Mechanism:** $\Delta\tau$ latency + finite tick-budget $B$.

**5. The "Infinite Acceleration" Paradox**  
*   **Classical Failure:** Certain geometric constraint configurations imply that acceleration diverges to infinity ($a \to \infty$).  
*   **SVET Resolution:** Acceleration is not a continuous vector; it is the emergent change in the rate of adjacency instantiations. Because the update rate is bounded by the local resolution latency $\Delta\tau$ and the absolute structural limit of $c$ (exactly one adjacency hop per tick), no infinite update rate can occur.  
*   **Mechanism:** Propagation Limit $c$ + $\Delta\tau$ latency.

**6. The Rigid-Rod Paradox (Instantaneous Force Transmission)**  
*   **Classical Failure:** A perfectly rigid rod transmits forces instantaneously across space, violating special relativity.  
*   **SVET Resolution:** There is no fundamental background geometry to support a rigid rod. A rod is an extended pattern with a finite resolution latency $\Delta\tau$; all constraint propagation is strictly limited by the node-set causal limit of $c$ (one adjacency hop per tick).  
*   **Mechanism:** STIP + adjacency-limited propagation.

**7. The "Simultaneous Constraint" Paradox**  
*   **Classical Failure:** Multiple simultaneous constraints produce contradictory force requirements that classical mechanics cannot resolve.  
*   **SVET Resolution:** The node ledger resolves each adjacency exaction locally and independently. Any global constraint contradictions are resolved in situ through Accounting Shock and $\Delta H$ diversion; no global simultaneity exists.  
*   **Mechanism:** Node Ledger Identity.

**8. The "Rigid Body Rotation" Paradox (Infinite Stress at Corners)**  
*   **Classical Failure:** Rigid polygons rotating at finite speed require infinite material stress at their outer corners.  
*   **SVET Resolution:** There are no physical corners. Coherence-constraint sets reconfigure their local directional asymmetries, with any unresolvable update demands shed into the $H$-channel as $\Delta H$ in high-gradient regions.  
*   **Mechanism:** Coherence-Constraint Reconfiguration + $\Delta H$ shedding.

**9. The "Non-Integrable Constraint" Paradox**  
*   **Classical Failure:** Non-holonomic constraints cannot be integrated into a globally consistent path of motion.  
*   **SVET Resolution:** Motion is not integrated mathematically; it is instantiated physically. Each tick is resolved locally and independently by the local update rules; there is no requirement for global integrability.  
*   **Mechanism:** STIP + discrete adjacency instantiation.

**10. The "Zero-Time Collision" Paradox**  
*   **Classical Failure:** Two bodies colliding in zero time require infinite reaction forces.  
*   **SVET Resolution:** Collisions require a finite resolution latency ($\Delta\tau > 0$). There are no zero-time events; the local ledger enforces a finite, capacity-limited update sequence.  
*   **Mechanism:** $\Delta\tau$ latency + finite tick-budget $B$.

**11. The "Infinite Regress of Constraints" Paradox**  
*   **Classical Failure:** Nested constraint chains imply an infinite spatial regress of action and reaction forces.  
*   **SVET Resolution:** There are no physical forces. There are only local adjacency exactions; there is no regress because each node resolves only the exactions originating within its immediate adjacency neighborhood.  
*   **Mechanism:** Locality + Adjacency Neighborhood.

**12. The "Rigid-Body Fracture Singularity" Paradox**  
*   **Classical Failure:** Linear elastic fracture mechanics predicts infinite stress singularities at sharp crack tips.  
*   **SVET Resolution:** Material stress is modeled as localized node strain $S(x)$. Because strain is strictly bounded by the available tick-budget $B$, no singularity can form; exceeding $B$ simply triggers $\Delta H$ shedding, causing the pattern to fracture cleanly.  
*   **Mechanism:** Bounded $S(x)$ + $\Delta H$ shedding.

**13. The "Instantaneous Reversal" Paradox**  
*   **Classical Failure:** A moving body reversing direction with no time delay requires infinite jerk.  
*   **SVET Resolution:** Reversal requires a finite resolution latency ($\Delta\tau$). No instantaneous updates are allowed; the local ledger enforces a finite, step-by-step reconstruction.  
*   **Mechanism:** $\Delta\tau$ latency + propagation limit $c$.

**14. The "Zero-Mass Constraint" Paradox**  
*   **Classical Failure:** Massless bodies under physical constraints produce undefined, singular accelerations.  
*   **SVET Resolution:** Massless patterns do not exist; all physical patterns possess a finite coherence-constraint set rigidity. Because rigidity is bounded, all accelerations remain finite and defined.  
*   **Mechanism:** Mass = constraint-set rigidity.

**15. The "Infinite Rigidity" Paradox**  
*   **Classical Failure:** Perfectly rigid bodies imply infinite material stiffness, requiring infinite impact forces.  
*   **SVET Resolution:** Infinite rigidity does not exist. Under update pressure, coherence-constraint sets reconfigure their directional asymmetries, and the ledger enforces a finite, cadence-limited update step.  
*   **Mechanism:** Coherence-Constraint Reconfiguration.

**16. The "Simultaneous Multi-Contact" Paradox**  
*   **Classical Failure:** Multiple simultaneous contacts produce mathematically contradictory force solutions.  
*   **SVET Resolution:** Each contact is resolved locally and independently by the node set's local update rules. Contradictions trigger Accounting Shock; no global force balance is evaluated or required.  
*   **Mechanism:** Node Ledger Identity.

**17. The "Rigid-Body Sliding and Rotation" Paradox**  
*   **Classical Failure:** Rigid bodies sliding and rotating simultaneously produce mathematically inconsistent constraints under classical friction laws.  
*   **SVET Resolution:** Sliding is modeled as directional decoherence, while rotation is modeled as coherence-constraint reconfiguration. The local update rules resolve each tick independently, eliminating any multi-constraint inconsistencies.  
*   **Mechanism:** $\Delta H$ shedding + STIP.

**18. The "Instantaneous Torque Transfer" Paradox**  
*   **Classical Failure:** Rotating rigid bodies transmit torque instantaneously across their radius, violating special relativity.  
*   **SVET Resolution:** Torque is modeled as a rotating directional asymmetry of exactions. Its propagation across the node set is limited by the causal ceiling $c$; no instantaneous transfer can occur.  
*   **Mechanism:** Adjacency-limited propagation.

**19. The "Rigid-Body Chain Reaction" Paradox**  
*   **Classical Failure:** A chain of rigid links transmits impulses instantaneously across its entire length.  
*   **SVET Resolution:** Each link in the chain has a finite resolution latency ($\Delta\tau$). No instantaneous chain propagation can occur; the node set enforces sequential, step-by-step updates.  
*   **Mechanism:** $\Delta\tau$ latency + propagation limit $c$.

**20. The "Non-Unique Contact Mode" Paradox**  
*   **Classical Failure:** Multiple mathematically valid contact modes produce non-unique, ambiguous force solutions.  
*   **SVET Resolution:** The local update rules deterministically select the unique adjacency path that minimizes the local coherence cost $C(x,v)$. A single, unique continuation path always emerges.  
*   **Mechanism:** Coherence-Minimal Continuation Path.

**21. The "Rigid-Body Jamming" Paradox**  
*   **Classical Failure:** Rigid bodies jam unpredictably due to mathematically inconsistent constraint requirements.  
*   **SVET Resolution:** Jamming is modeled as a local divergence of resolution latency ($\Delta\tau \to \infty$). The node set resolves the exaction conflict via Accounting Shock; no undefined states can occur.  
*   **Mechanism:** $\Delta\tau$ latency + local strain $S(x)$.

**22. The "Rigid-Body Corner Impact" Paradox**  
*   **Classical Failure:** Corner impacts on rigid bodies produce undefined force distributions.  
*   **SVET Resolution:** A corner is modeled as a high-curvature coherence-constraint set. The local update rules resolve the impact via $\Delta H$ shedding; no undefined force distributions are evaluated.  
*   **Mechanism:** $\Delta H$ shedding + Coherence-Constraint Reconfiguration.

**23. The "Rigid-Body Contact Singularity" Paradox**  
*   **Classical Failure:** Contact points between rigid bodies produce singular, infinite stress fields.  
*   **SVET Resolution:** Stress is modeled as local strain $S(x)$. Because $S(x)$ is strictly bounded by the available tick-budget $B$, no singularity can form; exceeding $B$ simply triggers $\Delta H$ shedding.  
*   **Mechanism:** Finite tick-budget $B$ + local strain $S(x)$.

**24. The "Rigid-Body Sliding Paradox"**  
*   **Classical Failure:** Sliding with friction produces contradictory force solutions in classical mechanics.  
*   **SVET Resolution:** Friction is not an active force; it is the directional coherence cost density $C(x,v)$ coupled with localized coherence-shedding ($\Delta H$). The local update rules resolve all contradictions deterministically.  
*   **Mechanism:** Coherence Cost Density $C(x,v)$ + $\Delta H$ shedding.

**25. The "Rigid-Body Non-Existence" Paradox**  
*   **Classical Failure:** Certain rigid-body configurations have no mathematically valid solutions.  
*   **SVET Resolution:** The node set's local update rules always resolve. Because no global force balance is required, there are no non-existent states.  
*   **Mechanism:** Node Ledger Identity.

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

## Appendix E: Coherence Manifold Toy Formulations

*The following forms are phenomenological toy models, not proposed as fundamental SVET laws; they are used to explore how utilization-driven metrics might reproduce GR-like behavior.*

### 1. Minimal Toy Formulations
We express the pattern-to-strain mapping tensor $\mathcal{F}_{ij}$, the strain-to-bias mapping $\mathcal{G}_a$, and the directional coherence cost density $\mathcal{H}$ as:
$$\mathcal{F}_{ij}[P] = \lambda_1 P \partial_i\partial_j P + \lambda_2 \partial_i P \partial_j P$$
$$\mathcal{G}_a[S] = \beta_a \mathrm{tr}(S) + \gamma_a S_{a}^{\;\;b}n_b$$
$$\mathcal{H}(B, v) = \kappa(B)\|v\|^2 + \mu(B)(v \cdot \hat{b})^2$$
where $\hat{b}$ is the local unit vector of update bias, and the scaling coefficients are defined relative to the localized processing budget:
$$\kappa(B) = \frac{\kappa_0}{1 + B}, \qquad \mu(B) = \mu_0 B$$

### 2. Parametric 2D Radial Metric Mapping
For a 2D polar slice ($r, \theta$) under a localized radial utilization field $U(r)$, the remaining budget is $B(r) = 1 - U(r)$. Setting the local bias magnitude $\kappa(B) = \kappa_0 / (2 - U(r))$ yields the emergent radial metric components:
$$g_{rr}(r) = 1 + \kappa(B) = 1 + \frac{\kappa_0}{2 - U(r)}$$
$$g_{\theta\theta}(r) = r^2 \big(1 + \mu(B)\big) = r^2 \big(1 + \mu_0 (1 - U(r))\big)$$
This defines a continuous, non-singular metric space where local utilization directly scales the spatial components, reproducing Schwarzschild-like deflection fields in the weak-limit.

### 3. Discrete Grid Solver Pseudocode ($\delta A = 0$)

---

© 2026 John Kirby. Licensed under the MIT License.
