This is the finalized **SVET Master Glossary v1.2.4**, formatted in clean Markdown with MathJax support. This document is ready to be committed to your `docs/` folder or appended to the `theory.md` file.

***

# SVET Master Glossary v1.2.4

This document serves as the authoritative notation reference for **Static Vacuum Excitation Theory (SVET)**. It defines the primitives of the node network and the derived quantities that emerge as classical physical observables.

## 1. Notation Table

| Symbol | Name | Type | Forensic Role |
| :--- | :--- | :--- | :--- |
| $B$ | **Budget** | Primitive | Maximum coherent update capacity per node per tick. |
| $S$ | **Strain** | Primitive | Incoming coherent update demand (load). **Invariant: $S \ge 0$.** |
| $\tau$ | **Local Cadence** | Primitive | Fundamental update timing of a node. |
| $\Xi$ | **Exaction** | Primitive | Residual continuity requirement imposed on neighbors. |
| $H$ | **H-channel** | Primitive | Ledger for collapsed/incoherent energy (heat, debris). |
| $B_0$ | **Floor Budget** | Primitive | Minimum coherent-processing capacity in the absence of load. |
| $c$ | **Max Prop. Rate** | Constant | One adjacency hop per substrate tick in vacuum. |
| $\tau_0$ | **Vacuum Cadence** | Constant | Baseline update timing in a zero-strain vacuum. |
| $\kappa_{yield}$ | **Yield Constant** | Constant | Threshold where demand exceeds pattern stability. |
| $\Delta\tau$ | **Resolution Latency** | Derived | Ticks required for a pattern to rebuild its coherent state. |
| $\tau_{eff}$ | **Effective Cadence** | Derived | Realized update timing under load or medium. |
| $m$ | **Mass** | Derived | Totality of node and adjacency complexity. |
| $E$ | **Energy** | Derived | Total update-budget required to maintain a pattern. |
| $v$ | **Velocity** | Derived | Adjacency hops per tick, constrained by $\Delta\tau$. |
| $a$ | **Acceleration** | Derived | Change in hops per tick as $\Delta\tau$ varies across space. |
| $U$ | **Utilization** | Ratio | Capacity utilization ratio ($U = S/B$). |
| $n$ | **Refractive Index** | Ratio | Ratio of $\tau_{eff} / \tau_0$. |
| $\eta$ | **Efficiency** | Ratio | Fraction of demand that becomes flux rather than $H$. |
| $\Gamma_p$ | **Pattern Stability** | Metric | Robustness of a pattern's coherence under strain. |
| $\ell_{adj}$ | **Adjacency Length** | Metric | Number of adjacency hops in a pattern’s footprint. |
| $\rho_{adj}$ | **Adjacency Density** | Metric | Adjacency constraints per unit pattern. |
| $\Omega_p$ | **Pattern Frequency** | Metric | Ticks per internal oscillation of a pattern. |
| $\Lambda$ | **Coherence Length** | Metric | Hops a pattern can propagate before decohering. |
| $\chi$ | **Excitation** | Config | Localized perturbations/disturbances in the network. |
| $\Phi$ | **Flux Count** | Config | Discrete count of coherent updates crossing an adjacency. |
| $\psi$ | **Pattern State** | Config | Full adjacency-coherent configuration at a specific tick. |

---

## 2. Detailed Definitions

### **B₀ — Floor Budget (Primitive)**
The minimum coherent-processing capacity a node possesses in the absence of strain or pattern load. 
*   **Note:** This is not a reservoir or "energy" source; it is a hardware permission that enables nodes to accept and retransmit coherent demand even when not already carrying a pattern.

### **U — Utilization (Ratio)**
The capacity utilization ratio, defined as $U = S/B$. It represents how much of a node’s capacity is currently consumed relative to its available budget. This is the primary diagnostic for redline detection and hardware/software audits.

### **Δτ — Resolution Latency (Derived)**
The measured number of global ticks required for a pattern to re-establish its adjacency-coherent state before it can propagate to the next node. $\Delta\tau$ is the physical mechanism behind time dilation and the refractive index.

### **χ — Chi (Config)**
Represents small, localized perturbations or disturbances in the node network that do not yet constitute a coherent update demand. Used for stress monitoring and local disturbance analysis.

### **Φ — Phi (Config)**
A discrete count of coherent update events successfully crossing an adjacency per tick. In SVET, $\Phi$ is strictly a count of events and is **not** related to gravitational potential.

### **a — Acceleration (Derived)**
The change in propagation rate (adjacency hops per tick) as Resolution Latency ($\Delta\tau$) varies across space. A pattern "accelerates" when it moves into a region where the node network can resolve its complexity in fewer ticks.

### **m — Mass (Derived)**
The derived totality of Node and Adjacency complexity. It accounts for the pattern's footprint ($\ell_{adj}$), its stability ($\Gamma_p$), and its required resolution time ($\Delta\tau$).

### **η — Efficiency (Ratio)**
The fraction of coherent update demand that successfully becomes flux rather than collapsing into the H-channel.

---

## 3. Rule-Level Mechanics (Accounting)

*   **Coherent Rejection:** A surface-level failure to accept update demand due to insufficient neighbor budget ($B$). This is the mechanism of reflection.
*   **Yield Event:** When the ratio of update demand to capacity ($S/B$) exceeds the pattern's stability ($\Gamma_p$), causing a collapse into the incoherent energy ledger ($H$).
*   **The Node Ledger:** The fundamental conservation identity:
    $$I_{in} = I_{refl} + I_{trans} + \Delta H = 100\%$$

---

© 2026 John Kirby. Licensed under the MIT License.
