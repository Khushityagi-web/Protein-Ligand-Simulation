# Molecular Docking and Molecular Dynamics Simulation of Erlotinib with EGFR
A Computational Approach to Cancer Therapeutics

## Project Overview

This project investigates the interaction between **Erlotinib**, a tyrosine kinase inhibitor, and the **EGFR** receptor using molecular docking and molecular dynamics (MD) simulation.  
The goal is to understand binding affinity, complex stability, and structural changes.  
Steps were performed manually during learning; workflow notes are included.

---

## Repository Structure

```
Protein-Ligand-Simulation/
│
├── Docking/
│   ├── receptor/
│   │   └── REC.pdb
│   ├── ligand/
│   │   ├── LIG_sp.pdb
│   │   └── LIG.mol2
│   └── docking_results/
│       └── bestcomplex.pdbqt
│
├── MD_Simulation/
│   ├── input_files/
│   │   ├── box.gro
│   │   ├── box_sol.gro
│   │   ├── box_sol_ion.gro
│   │   ├── topol.top
│   │   └── ions.mdp
│   └── outputs/
│       ├── EM.gro
│       ├── EM.edr
│       ├── EM.log
│       ├── NVT.gro
│       ├── NVT.cpt
│       ├── NPT.gro
│       ├── NPT.cpt
│       ├── MD.tpr
│       ├── MD.xtc
│       └── MD_center.xtc
│
├── MD_Simulation_Scripts/
│   (workflow notes)
│
├── Post-MD Simulation Assessment/
│   (analysis placeholders)
│
└── Visulizations and Results.pdf
```

---

## Input Files

- **LIG_sp.pdb** – prepared ligand  
- **LIG.mol2** – optimized ligand  
- **REC.pdb** – receptor  
- **box.gro** – simulation box  
- **box_sol.gro** – solvated system  
- **box_sol_ion.gro** – ionized solvated system  
- **topol.top** – topology  
- **ions.mdp** – ion parameter file  

---

## MD Output Files

- **Energy Minimization:** EM.gro, EM.edr, EM.log  
- **NVT Equilibration:** NVT.gro, NVT.cpt  
- **NPT Equilibration:** NPT.gro, NPT.cpt  
- **Production MD:** MD.tpr, MD.xtc, MD_center.xtc  

Visualization outputs are included in **Visulizations and Results.pdf**.

---

## Tools and Software Used

### Structure Preparation
PyMOL  
ChimeraX  
AutoDock Tools  
Avogadro  
SwissParam  
BIOVIA Discovery Studio  

### Docking & Simulation
AutoGrid  
AutoDock  
GROMACS  
VMD  
XMGrace  

### ADMET & Toxicity
SwissADME  
PROTox-3  
SwissTargetPrediction  

---

## Workflow Summary

### 1. Protein & Ligand Preparation
Cleaning, hydrogens, optimization, force field parameters.

### 2. Molecular Docking
Grid definition, docking, and pose selection.

### 3. Molecular Dynamics Simulation
Box setup → solvation → ions → EM → NVT → NPT → production MD.

### 4. Post-MD Analysis
RMSD, RMSF, hydrogen bonds, energy analysis, trajectory correction.

### 5. ADMET & Toxicity
Drug-likeness and toxicity assessment.

---

## Key Results

- Stable docking pose  
- RMSD & RMSF show stable dynamics  
- Hydrogen bonds stay consistent  
- Energy profiles confirm proper equilibration  

---

## Future Improvements

- Add executable `.sh` / `.py` scripts  
- Add `.xvg` files  
- Implement MM/PBSA  
- Add more plots and comparative results  
