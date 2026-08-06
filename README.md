# In Silico Exploration of *Berberis lycium* Phytochemicals as Potential Inhibitors of CHIKV Receptors (nsp1, nsp2, and nsp3)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![GROMACS](https://img.shields.io/badge/MD%20Simulation-GROMACS-blue)](https://www.gromacs.org/)
[![PyRx](https://img.shields.io/badge/Docking-PyRx%2FAutoDock%20Vina-green)](https://pyrx.sourceforge.io/)

## Project Overview
Computational screening and 10 ns Molecular Dynamics (MD) evaluation of bio-active phytochemicals; Berberine and Palmatine, derived from *Berberis lycium* against critical non-structural replication proteins (nsp1, nsp2, nsp3) of Chikungunya Virus (CHIKV).

---

## 🔬 Methodology Overview

### 1. Data Collection & Target Preparation
* **Target Retrieval & Refinement:** Three-dimensional structural coordinates for Chikungunya virus (CHIKV) replication proteins were retrieved from the RCSB Protein Data Bank (PDB):
  * **nsP1 Capping Enzyme:** [PDB ID: 6Z0V](https://www.rcsb.org/structure/6z0v) (2.60 Å Cryo-EM resolution). To resolve computational overhead from the full 12-mer dodecameric assembly, a single functional protomer (**Chain A**) was isolated to represent the active catalytic site.
  * **nsP2 Protease:** [PDB ID: 4ZTB](https://www.rcsb.org/structure/4ZTB) (X-ray diffraction structure processed as a full functional monomer).
  * **nsP3 Macrodomain:** [PDB ID: 4ZTB](https://www.rcsb.org/structure/4ZTB) (X-ray diffraction structure containing the conserved ADP-ribose binding domain).
* **Receptor Clean-up:** Target structures were processed using BIOVIA Discovery Studio and PyMOL to remove water molecules, heterogens, and non-standard ions, resolve alternate location conformers, and repair missing residues prior to conversion into `.pdbqt` format.
* **Ligand Library Construction & Optimization:** 
  * Core isoquinoline alkaloids were retrieved in 3D SDF/PDB format: **Berberine** from [DrugBank (DB04115)](https://go.drugbank.com/drugs/DB04115) and **Palmatine** from [PubChem (CID: 19009)](https://pubchem.ncbi.nlm.nih.gov/compound/19009).
  * Ligands underwent energy minimization (UFF force field) and partial charge assignment inside PyRx prior to conversion into `.pdbqt` format for virtual screening.
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
| **nsp1** | Berberine | -10.7 | X.XX nm |
| **nsp2** | Berberine | -9.0 | X.XX nm |
| **nsp3** | Berberine | -11.5 | X.XX nm |
| **nsp1** | Palmatine | -8.2 | X.XX nm |
| **nsp2** | Palmatine | -7.6 | X.XX nm |
| **nsp3** | Palmatine | -9.2 | X.XX nm |

---

## Pose Visualizations

