# In Silico Exploration of *Berberis lycium* Phytochemicals as Potential Inhibitors of CHIKV Receptors (nsp1, nsp2, and nsp3)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![GROMACS](https://img.shields.io/badge/MD%20Simulation-GROMACS-blue)](https://www.gromacs.org/)

## Project Overview
Computational screening and 10 ns Molecular Dynamics (MD) evaluation of bio-active phytochemicals derived from *Berberis lycium* against critical non-structural replication proteins (nsp1, nsp2, nsp3) of Chikungunya Virus (CHIKV).

---

## 🔬 Methodology Overview

### 1. Data Collection & Preparation
- **Target Retrieval:** PDB structures acquired and processed (water molecules and heterogens removed, missing loops repaired).
- **Ligand Library:** Phytochemicals retrieved from PubChem, energy-minimized, and converted for docking.

### 2. Molecular Docking & Interaction Analysis
- **Grid Configuration:** Site-specific grid boxes constructed around active site residues of nsp1, nsp2, and nsp3.
- **Visual Profiling:** 2D interaction maps (H-bonds, hydrophobic, pi-stacking) and 3D surface binding poses.

### 3. ADMET & Pharmacokinetics
- Drug-likeness evaluation via Lipinski's Rule of Five, bioavailability radar, and toxicity profiles.

### 4. Molecular Dynamics Simulation (10 ns)
- Solvated in TIP3P water box with neutralizing counter-ions using GROMACS.
- Stability evaluated via RMSD, RMSF, Rg, and Hydrogen Bond longevity profiles.

---

## Key Results

| Target | Lead Phytochemical | Binding Affinity (kcal/mol) | 10 ns RMSD (Average) |
| :--- | :--- | :--- | :--- |
| **nsp1** | Berberine | -X.X | X.XX nm |
| **nsp2** | Berberine | -9.0 | X.XX nm |
| **nsp3** | Berberine | -11.5 | X.XX nm |
| **nsp1** | Palmatine | -X.X | X.XX nm |
| **nsp2** | Palmatine | -X.X | X.XX nm |
| **nsp3** | Palmatine | -X.X | X.XX nm |

---

## Pose Visualizations

