# Pancreatic Alpha-Amylase Docking with Curcumin, Berberine, and Berbamine
This repository contains a project focused on receptor-based drug design, where we perform molecular docking of pancreatic alpha-amylase (PDB ID: 1HNY) with three compounds: curcumin, berberine, and berbamine. The goal is to investigate the interaction of these ligands with the enzyme using AutoDock and analyze the docking results to assess their potential as inhibitors of pancreatic alpha-amylase.

Project Overview
Pancreatic alpha-amylase plays a significant role in carbohydrate digestion. Inhibitors of this enzyme are of interest for managing diabetes by slowing the breakdown of carbohydrates into sugars. This project explores the binding affinity of curcumin, berberine, and berbamine—compounds known for their potential biological activities—against pancreatic alpha-amylase.

Ligands:
Curcumin: A polyphenolic compound found in turmeric, known for its anti-inflammatory and antioxidant properties.
Berberine: An alkaloid extracted from several plants, with antimicrobial and anti-inflammatory effects.
Berbamine: A compound derived from the Berberis genus, with potential therapeutic effects in various diseases, including cardiovascular and inflammatory conditions.
Receptor:
Pancreatic Alpha-Amylase (PDB ID: 1HNY): An enzyme that catalyzes the hydrolysis of starch into sugars. Inhibiting this enzyme can potentially help in the management of diabetes and metabolic disorders.
Installation
To set up the project and run the molecular docking simulations, ensure the following dependencies are installed:

AutoDock: For performing molecular docking.
Open Babel: For converting between file formats.
RDKit: For generating SMILES representations and calculating molecular properties.
Biopython: For handling protein structures.
py3Dmol: For visualizing the docking results.
Matplotlib: For plotting any relevant graphs.
Docking Procedure
The docking was performed using the following steps:

Ligand Preparation: The three ligands (curcumin, berberine, and berbamine) were converted into 3D structures using Open Babel and prepared in PDBQT format, which is required by AutoDock.

Receptor Preparation: The receptor (pancreatic alpha-amylase, PDB ID: 1HNY) was processed and converted into the appropriate format (PDBQT) for docking.

Docking Simulation: AutoDock4.2 was used to perform the docking. We defined the grid box around the receptor’s active site to focus the docking on potential binding regions.

Results Extraction: The docking results were analyzed by extracting key parameters such as binding energy, inhibition constant, ligand efficiency, and vdW + H-bond + desolvation energies.

Visualization: The protein-ligand interactions were visualized using py3Dmol, providing insights into the binding poses and interactions.

Key Parameters in Docking Results
The following parameters were extracted from the AutoDock docking log files:

Binding Energy (ΔG):

Represents the free energy of binding between the ligand and the receptor.
A more negative binding energy indicates a stronger interaction between the ligand and the receptor.
This value is crucial for predicting the affinity of the ligand to the receptor. Lower (more negative) binding energies are generally preferred, indicating tighter binding.
Inhibition Constant (Ki):

Reflects the concentration of ligand needed to inhibit the enzyme by half.
Lower values of Ki indicate more potent inhibitors.
A smaller Ki suggests that the compound has a high binding affinity for the enzyme.
Ligand Efficiency:

This is a measure of how efficiently the ligand binds to the target, considering its molecular size. It is calculated as the ratio of binding energy to the number of heavy atoms in the ligand.
Ligands with high ligand efficiency tend to be more effective, as they require fewer atoms to bind tightly to the receptor.
vdW + H-bond + Desolvation Energy:

This term represents the total non-covalent interaction energy between the ligand and the receptor.
It includes contributions from van der Waals interactions, hydrogen bonds, and the desolvation energy (energy required to displace water molecules from the binding site).
A lower (more negative) value indicates better overall binding due to favorable non-covalent interactions.
These docking studies suggest that these compounds could be further explored in vitro to evaluate their potential as pancreatic alpha-amylase inhibitors, with curcumin standing out as a particularly promising candidate due to its better binding affinity.

Future Work
In vitro validation: Perform enzyme inhibition assays to validate the in silico findings.
Dynamic simulations: Perform molecular dynamics simulations to better understand the stability of the ligand-receptor interactions over time.
Optimization: Modify the structures of these ligands to improve binding affinity and specificity.
