# SVET Master Glossary v1.2.6

This document serves as the authoritative notation and terminology reference for **Static Vacuum Exaction Theory (SVET)**.

---

# SVET Authoritative Glossary

## Vocabulary
*This section serves as the centralized repository for the structural terms, local transaction mechanics, and environmental definitions unique to Static Vacuum Exaction Theory (SVET).*

---

## Mathematics & Symbolic Variables
*This section contains the formal mathematical primitives, operators, and coordinate-agnostic tensor notations used across the SVET master framework.*

---

## 1. Primitives (The Vacuum "Hardware")

### Node Set
**Type:** Primitive  
**Definition:** The fundamental, static ensemble of discrete update sites (nodes) with fixed adjacency relations and local update rules.  
**Forensic Role:** Serves as the primary, non-coordinate space of the universe. It completely replaces legacy mechanical terms ("substrate") and wired computational terms ("network"). Emergent spacetime, continuous geometry, and fields are represented as dynamic routing configurations across this static set.

### $B$ — "Budget"
**Type:** Primitive  
**Definition:** Maximum coherent update capacity of a node per tick.  
**Forensic Role:** Represents the "fuel" available for pattern re-instantiation.

### $S$ — "Strain"
**Type:** Primitive  
**Definition:** Incoming coherent update demand (load).  
**Invariant:** $S \ge 0$.  
**Forensic Role:** Represents the "work" currently placed on a node.

### $\tau$ — "tau"
**Type:** Primitive  
**Definition:** Local update timing (heartbeat) of a node.  
**Forensic Role:** The fundamental clock speed of the node set at a specific site.

### $\Xi$ — "Xi"
**Type:** Primitive  
**Definition:** Residual continuity requirement a node imposes on neighbors after its own update.  
**Forensic Role:** Mechanism of forward propagation and temporal continuity.

### $H$ — "H-channel"
**Type:** Primitive  
**Definition:** Incoherent energy ledger for collapsed update demand.  
**Forensic Role:** Captures "accounting debris" such as heat, fluorescence, and fracture.

---

## 2. Constants (Structural Invariants)

### $c$ — "c"
**Type:** Constant  
**Definition:** The invariant adjacency‑hop rate of the node space; the maximum rate at which coherent influence, strain, or routing information can propagate between adjacent nodes.  
**Forensic Role:** Structural causal ceiling of the node space; defines the maximum propagation rate of coherent updates and establishes the causal ordering of all pattern‑level dynamics.

### $\tau_0$ — "tau-naught"
**Type:** Constant  
**Definition:** Baseline update timing in a zero-strain vacuum.  
**Forensic Role:** Reference "heartbeat" for velocity and dilation calculations.

### $\kappa_{yield}$ — "kappa-yield"
**Type:** Constant  
**Definition:** Threshold constant defining when scaled demand exceeds pattern stability.  
**Forensic Role:** The "Redline" where a coherent pattern must fracture into the H-channel.

---

## 3. Derived Quantities (The "Observables")

### $\Delta\tau$ — "Delta-tau"
**Type:** Derived  
**Definition:** Number of global ticks required for a pattern to re-establish its adjacency-coherent state.  
**Logic:** Derived from $\tau, S, B, \Gamma_p,$ and CaBS.  
**Forensic Role:** Physical mechanism behind time dilation and refractive index.
*   **Emergent Interpretation:** Spatial variations in $\Delta\tau$ produce the timing gradients historically described as "ground-state tilt," giving rise to gravitational redshift, lensing, and time dilation.

### $\tau_{eff}$ — "tau-eff"
**Type:** Derived  
**Definition:** Realized update timing of a node under medium or load.  
**Forensic Role:** The "Slowed Heartbeat" observed in gravity wells or glass.

### $a$ — "a"
**Type:** Derived  
**Definition:** Change in propagation rate (adjacency hops per tick) caused by spatial variation in $\Delta\tau$.  
**Clarification:** Influenced by $\Delta\tau$ gradients but **not** equal to $d(\Delta\tau)/dx$.  
**Forensic Role:** SVET equivalent of acceleration; change in propagation behavior due to latency gradients.

### $v$ — "v"
**Type:** Derived  
**Definition:** Adjacency hops per tick, constrained by $\Delta\tau$.  
**Forensic Role:** Emergent velocity; how fast a pattern satisfies its own constraints.

### $m$ — "mass"
**Type:** Derived  
**Definition:** Totality of Node and Adjacency complexity.  
**Logic:** $m = f(\ell_{adj}, \Gamma_p, \Delta\tau)$.  
**Forensic Role:** Explains inertia as the "paperwork" required to move a complex pattern.

### $E$ — "energy"
**Type:** Derived  
**Definition:** Total coherent update-budget required per tick to maintain a pattern.  
**Forensic Role:** The "Operating Cost" of a pattern's existence.

### $\chi$ — "Chi"
**Type:** Derived  
**Definition:** Localized perturbations or disturbances that do not yet constitute coherent demand.  
**Forensic Role:** Monitors small-scale node set jitter and stress.  
**Clarification:** **Not** a demand channel; does **not** contribute to $S$.

### $B_0(x)$ — "Local Floor Budget"
**Type:** Local Parameter (Spatially Dependent)  
**Definition:** The minimum available tick-budget a node at coordinate $x$ must expend to participate in the vacuum of adjacency (to exist as a structural element of adjacency and tick-budget) [1].  
**Forensic Role:** Serves as the baseline structural existence cost of a node [1]. It represents pure, localized network structure induced entirely by the cumulative background exaction environment of the universe, rather than an independent energy reservoir or background field [1].

---

## 4. Ratios & Metrics (The "Diagnostics")

### $U$ — "Utilization"
**Type:** Ratio  
**Definition:** Capacity utilization ratio, $U = S/B$.  
**Forensic Role:** Measures how much of a node's capacity is consumed; used for redline detection.

### $n$ — "Refractive Index"
**Type:** Ratio  
**Definition:** $n = \tau_{eff} / \tau_0$.  
**Forensic Role:** Measures the "Lag" of light in a medium compared to vacuum.

### $\eta$ — "eta"
**Type:** Ratio  
**Definition:** Efficiency; fraction of coherent demand that becomes flux rather than $H$.  
**Forensic Role:** Measures the "Tax" or "Leakage" of an update.

### $\Gamma_p$ — "Gamma-p"
**Type:** Metric  
**Definition:** Pattern Stability Factor; robustness of a pattern's coherence under strain.  
**Forensic Role:** Determines if a pattern is a "Robust Loop" (particle) or a "Fragile Wave."
*   **Emergent Interpretation:** Historically referred to as "pattern rigidity." When the ratio $S_p/B$ exceeds $\kappa_{\text{yield}}\Gamma_p$, the pattern undergoes structural failure ("coherence catastrophe") and sheds energy into the incoherent channel ($H$).

### $\ell_{adj}$ — "ell-adj"
**Type:** Metric  
**Definition:** Adjacency Length; number of hops in a pattern's spatial footprint.  
**Forensic Role:** Defines the "Size" of a pattern in the node sets.

### $\Omega_p$ — "Omega-p"
**Type:** Metric  
**Definition:** Pattern Frequency; ticks per internal oscillation of a pattern.  
**Forensic Role:** The "Internal Clock" of a wave or particle loop.

### $\Lambda$ — "Lambda"
**Type:** Metric  
**Definition:** Coherence Length; hops a pattern can propagate before decohering into $H$.  
**Forensic Role:** Measures the "Life Expectancy" of a coherent signal.

---

## 5. Configurations & Accounting

### $\psi$ — "psi"
**Type:** Config  
**Definition:** Full adjacency-coherent configuration of a pattern at a specific tick.  
**Forensic Role:** The "Snapshot" of a pattern's state.

### $\Phi$ — "Phi"
**Type:** Discrete  
**Definition:** Count of coherent update events successfully crossing an adjacency per tick.  
**Note:** Not gravitational potential.  
**Forensic Role:** Measures the "Traffic" of coherent information.

### The Node Ledger
**Type:** Accounting Identity  
**Definition:** Conservation of exaction:  
$$I_{\text{in}} = I_{\text{refl}} + I_{\text{trans}} + \Delta H = 100\%$$

---

© 2026 John Kirby. Licensed under the MIT License.
