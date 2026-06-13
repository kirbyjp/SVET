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
