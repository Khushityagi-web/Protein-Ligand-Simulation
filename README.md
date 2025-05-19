# Molecular Docking and Dynamics Simulation of Erlotinib with EGFR: A Computational Approach to Cancer Therapeutics
#  Project Overview
This mini-project focuses on the molecular docking and molecular dynamics (MD) simulation of Erlotinib, a well-known tyrosine kinase inhibitor, with epidermal growth factor receptor (EGFR). The study aims to explore the binding interactions, stability, and conformational changes of the Erlotinib-EGFR complex to provide insights into its therapeutic potential in cancer treatment.

# Repository Contents
MD_Simulation_Scripts – Molecular docking script, docking protocol, and docking results.
Post-MDSimulation Assessment – Input and output files for molecular dynamics simulations, including configuration files and trajectory data. Python scripts for post-MD analysis, including RMSD, RMSF, hydrogen bonding, and binding energy calculations.
README.md - Project Description, Overview and instructions for using this repository.

# Input Files:
Ligand structure file: LIG_sp.pdb 
Receptor structure file: REC.pdb 
Simulation box file: box.gro 
Solvated system file: box_sol.gro
Topology file: topol.top 
Ion addition parameter file: ions.mdp 
Ionized solvated system file: box_sol_ion.gro 

# Molecular Dynamics Output Files: 
Energy Minimization: EM.gro,EM.log,EM.edr
NVT Equilibration: NVT.gro, NVT.cpt
NPT Equilibration: NPT.gro, NPT.cpt 
MD Simulation: MD.tpr, MD.xtc, MD_center.xtc
Visulization and Results

# Tools and Software:
Structure Preparation:
PyMOL: Converts ligand structures (SDF to PDB). Ensures compatibility.
ChimeraX: Cleans protein structures (removes water molecules). Prepares for docking.
AutoDock Tools (ADT): Prepares protein and ligand for docking (adds hydrogens, assigns charges).
Avogadro: Optimizes ligand structures for accuracy.
SwissParam: Generates force field parameters for small molecules.
BIOVIA Discovery Studio: Analyzes molecular interactions.
Docking and MD Simulation:
AutoGrid & AutoDock: Defines grid and predicts binding pose of Erlotinib.
GROMACS: Conducts molecular dynamics simulations.
VMD: Visualizes MD trajectories.
xmgrace: Plots RMSD and energy data.
ADMET and Toxicity Prediction:
SwissADME: Predicts ADME properties.
PROtox 3.0: Assesses toxicity profiles.

# Workflow Summary:
1. Protein & Ligand Preparation: Retrieve structures, clean, add charges, optimize ligand.
2. Molecular Docking: Define grid, dock ligand, analyze binding interactions.
3. Molecular Dynamics Simulation: Setup system, energy minimization, equilibration (NVT/NPT), run MD.
4. Post-Simulation Analysis: Compute RMSD, RMSF, hydrogen bonds, energy profiles.
5. ADMET & Toxicity Prediction: Evaluate drug-likeness and safety profile of Erlotinib.
6. Target Prediction: Identify biological targets using SwissTarget Prediction.
This streamlined workflow ensures efficient docking and simulation analysis of Erlotinib with EGFR.

# Key Results
Binding Affinity: Docking score analysis
Complex Stability: RMSD and RMSF analysis
Hydrogen Bonding: Interaction insights
