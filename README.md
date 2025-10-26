# Convex Optimization via Semidefinite Relaxations (SDR)

## About
This repository contains a compact project on applying **Semidefinite Relaxation (SDR)** to classic non-convex problems:
- **MIMO detection** (communications)
- **Max-Cut** (combinatorial optimization)
- **Graph coloring** (chromatic number bounds and algorithms)

It includes a self-contained **project report** and two executable notebooks. The report presents the derivations and algorithms; the notebooks reproduce core experiments and visualizations.

> 📄 See the full report: **[convex_project_report.pdf](convex_project_report.pdf)**



### What’s inside (brief)
- **MIMO Detection (SDR vs. ZF/MMSE/SD)**  
  Real-valued QCQP formulation → SDP relaxation → randomized recovery; BER vs. SNR and runtime scaling.  
  *Notebook:* `project-mimo.ipynb`
- **Max-Cut (SDP + Goemans–Williamson rounding)**  
  Laplacian form → SDP relaxation → **random hyperplane** rounding; cut quality vs. baselines on sample graphs.  
  *Notebook:* `MaxCut_GraphColoring.ipynb`
- **Graph Coloring (SDP & Lovász number; refined KMS)**  
  SDP surrogates for χ(G); **Lovász θ(G)** as a bound; hyperplane-based semi-colorings combined with degree-based peeling (Karger–Motwani–Sudan) for improved color counts.  
  *Notebook:* `MaxCut_GraphColoring.ipynb`

> Each section in the report mirrors the notebook logic and provides the math behind the implementations.
