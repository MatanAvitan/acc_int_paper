# Appendix: Geometric Foundation and Broad Sweeps

This document maps geometry-heavy material from `PAPER.md` to its intended destination in the manuscript appendix. These sections provide the empirical grounding for the manifold-aware erasure narrative by characterizing the representation space of Qwen2.5-0.5B.

## Mapping of Geometry Blocks

| PAPER.md Section | Appendix Destination | Key Content |
|------------------|----------------------|-------------|
| **3. Experiment 1: Subspace Projection (Q1)** | `Appendix~\ref{app:subspace}` | Subspace sufficiency (Q1), top-1 agreement vs. projection rank, layer-23 cliff. |
| **4. Experiment 2: Directional Perturbation (Q2)** | `Appendix~\ref{app:curvature}` | Manifold vs. flat subspace (Q2), on-subspace vs. off-subspace KL divergence ratios. |
| **5. Experiment 3: Representation Connectivity (Q3)** | `Appendix~\ref{app:connectivity}` | Shared vs. domain-specific manifolds (Q3), cluster analysis, interpolation smoothness. |
| **6. Experiment 4: Simultaneous Multi-Layer Projection (Q1-multi)** | `Appendix~\ref{app:multilayer}` | Multi-layer accumulation, graceful degradation, boundary exclusion (layers 1 and 23). |
| **7.1 Summary of Findings (Geometric)** | `Appendix~\ref{app:summary}` | Summary of linear subspace sufficiency, sensitivity concentration, and topology. |

## Retained Material for Appendix

The following broad sweeps and diagnostic results are moved to the appendix to keep the main text focused on the `gce_tangent` vs. `gce_ambient` comparison:

- **Broad Dataset Sweeps**: All results for Math (GSM8K) and Code (codeparrot) datasets.
- **Detailed Layer Passes**: Full sweep tables for layers {4, 8, 16, 23} across all metrics (Top-1, Top-5, KL, Cosine).
- **Cluster Analysis**: Silhouette scores and best-k results for all layer-dataset conditions.
- **Interpolation Curves**: Full midpoint metrics and interpolation curves for Sycophancy and Safety.
- **Multi-Layer Configurations**: Detailed results for expanding-from-middle and strided projection configurations.

## Verification Notes

- Main text `results.tex` and `experiments.tex` already contain references to these appendix labels.
- The narrative in the main text now prioritizes Sycophancy, Safety, and Bias in Bios as the primary evidence path.
- Geometry material remains available as supporting evidence for the "off-manifold displacement" claim.
