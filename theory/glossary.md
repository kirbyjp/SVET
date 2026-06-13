# SVET Master Glossary v1.2.6

This document serves as the authoritative notation and terminology reference for **Static Vacuum Excitation Theory (SVET)**.

---

## 1. Primitives (The Substrate "Hardware")

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
**Forensic Role:** The fundamental clock speed of the substrate at a specific site.

### $\Xi$ — "Xi"
**Type:** Primitive  
**Definition:** Residual continuity requirement a node imposes on neighbors after its own update.  
**Forensic Role:** Mechanism of forward propagation and temporal continuity.

### $H$ — "H-channel"
**Type:** Primitive  
**Definition:** Incoherent energy ledger for collapsed update demand.  
**Forensic Role:** Captures "accounting debris" such as heat, fluorescence, and fracture.

### $B_0$ — "B-zero"
**Type:** Primitive  
**Definition:** Minimum coherent-processing capacity a node possesses in the absence of load.  
**Forensic Role:** Hardware permission enabling nodes to transmit demand even when "idle."  
**Clarification:** **Not** vacuum energy, dark energy, stored energy, or a cosmological reservoir.

---

## 2. Constants (The Substrate "Laws")

### $c$ — "c"
**Type:** Constant  
**Definition:** Maximum propagation rate; exactly one adjacency hop per substrate tick in vacuum.  
**Forensic Role:** Universal speed limit of the hardware.

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
**Forensic Role:** Monitors small-scale substrate jitter and stress.  
**Clarification:** **Not** a demand channel; does **not** contribute to $S$.

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
**Forensic Role:** Defines the "Size" of a pattern in the node network.

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
$$I_{in} = I_{refl} + I_{trans} + \Delta H = 100\%$$

---

© 2026 John Kirby. Licensed under the MIT License.
