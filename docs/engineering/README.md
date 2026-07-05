# SVET Engineering Governance

This directory contains the developer workflow documentation, software engineering standards, and baseline-preservation guardrails for the Static Vacuum Excitation Theory simulation engines.

---

### TODO: Integrate AIstudio Guardrails and Baseline Preservation Workflow  
(See `SVET_issues_list.xls` — Tab “SVET Code Workflow / AIstudio Guardrails”)

The v0.07.3 baseline-preservation protocol, pull request (PR) workflow, protected markers, and precommit hooks have been reviewed and archived. These items govern how AIstudio and Dev assistants interact with the SVET codebase and must be incorporated into the engineering documentation once the v0.07.4 patch cycle stabilizes.

### TODO: Coherence Manifold Simulation Implementation (See `SVET_issues_list.xls` — Tab “Coherence Manifold”)

*   Incorporate the 2D radial metric mapping equations from Appendix E into the lattice simulation engine.
*   Configure the solver to run parameter sweeps mapping CSV audit fields (horizon radius, utilization $U(r)$, and directional bias) to the parameters in the toy functions $\mathcal{F}$, $\mathcal{G}$, and $\mathcal{H}$.
*   Validate the emergent least-cost paths against active grid runs and implement logging for the following active diagnostics:
    *   `nodes_biased_count`: The count of nodes per update step where utilization exceeds the background floor ($U(r) > U_{\text{floor}}$).
    *   `nodes_skipped_count`: The count of nodes bypassed per iteration when local update latency ($\tau_{\text{eff}}$) exceeds maximum processing limits.

---

### TODO: Universal Horizon Axis Selector and Universality Scoring Suite (See `SVET_issues_list.xls` — Tab “Coherence Manifold”)

*   Implement an interactive selector row in the monitor interface to toggle the horizontal plotting axis ($x$-axis) between the following six candidate universal variables:
    1.  **Normalized Radius:** $r / r_{\text{hor}}$ (Proximity to the Schwarzschild horizon)
    2.  **Dimensionless Potential:** $\Phi = \frac{GM}{r c^2}$ (Local gravitational well depth)
    3.  **Normalized Excitation:** $S_{\text{norm}} = \frac{\eta}{\eta_{\text{max}}}$ (Local node network strain)
    4.  **Cosmic Coherence:** $C = \tau_{\text{eff}} H_0$ (Cosmic expansion suppression factor)
    5.  **Composite Axis:** A user-weighted, parameterized blend of the above candidate variables.
    6.  **Null Option:** Raw physical radius ($r$) and raw parameter dials.
*   Develop the **Universality Scoring Algorithm** to calculate and report the following real-time metrics for each selected plotting axis across mass sweeps (proton $\to$ Sun $\to$ Neutron Star $\to$ Black Hole):
    *   **Curve Collapse Score:** Quantifies the mathematical convergence (overlay tightness) of different mass curves on the active axis.
    *   **Monotonicity and Smoothness Scores:** Detects and penalizes any step-function jumps or non-monotonic behavior along the active axis.
    *   **GR Compatibility Score:** Measures the deviation between the SVET curve and classical GR in the weak-field regime ($U \to 0$), ensuring the axis correctly aligns the trusted classical tails.
    *   **QG Compatibility Score:** Evaluates whether the SVET curves consistently peel away from GR to approach flat-line saturation ($U \to 1$) in the strong-field quantum regime.
*   Validate the emergent least-cost paths against active grid runs and implement logging for the following active diagnostics:
    *   `nodes_biased_count`: The count of nodes per update step where utilization exceeds the background floor ($U(r) > U_{\text{floor}}$).
    *   `nodes_skipped_count`: The count of nodes bypassed per iteration when local update latency ($\tau_{\text{eff}}$) exceeds maximum processing limits.
 
---

###Tool specific scoring metrics

### Forensic Diagnostic Invariants

The following metrics are tool-specific diagnostic scores used by the CaBS Forensic Monitor to evaluate the stability and universality of candidate exaction models [1].

#### $I_C$ — "Cosmic Correspondence Score"
**Type:** Diagnostic Metric  
**Definition:** Quantifies how accurately the SVET exaction-potential ($\Psi$) matches the observed Hubble expansion at a given radius [1]. A value of $1.0$ indicates a perfect cosmological match.

#### $I_S$ — "Saturation Safety Score"
**Type:** Diagnostic Metric  
**Definition:** Measures the available budget headroom of the node set to ensure the interior remains protected from premature cadence-freezing [1]. A value of $1.0$ indicates optimal structural stability.

#### $I_L$ — "Local Ledger Load Score"
**Type:** Diagnostic Metric  
**Definition:** Tracks the cumulative "update debt" (accumulated exaction-strain) as the evaluation frame moves toward a high-density core [1].

#### $N$ — "Local Capacity Ratio"
**Type:** Diagnostic Metric  
**Definition:** The ratio of hardware-level node update cycles available per pattern-level software update [1]. Higher values indicate greater resolution safety for complex patterns.
