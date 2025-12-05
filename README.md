# Dipeptides-wB9M-V Dataset  
Geometry-Optimized Dipeptides and AMI/Distance Analysis Files

This repository contains the full dataset of dipeptides used in the mutual information (MI) benchmarking study. Each dipeptide was geometry optimized and analyzed using density functional theory (DFT) on top of semi-empirical methods. The directory structure is organized by amino-acid pair (e.g., ALAALA, ALAARG, ALAASN).

## Computational Methods
All dipeptides were geometry optimized using a two-step procedure:  
1. Initial optimization with AM1 and PM3.  
2. Final optimization at the B3LYP level of theory.  

AMI matrices, entropy values, and distance-based descriptors were extracted from the optimized structures.

## Repository Structure

Each dipeptide folder contains files in the following format:

- `NAME.xyz` — Final B3LYP-geometry optimized Cartesian coordinates  
- `NAME-I_ij.csv` — Orbital mutual information matrix  
- `NAME-I_ij_sum.csv` — Atomic mutual information matrix   
- `NAME-atomic-s1.csv` — Atomic entropies  
- `NAME-ANG_distance.csv` — Atom pair distance matrix (Å)  
- `NAME-figure.svg` — SPatial Atom-Wise Network (SPAWN) plot for AMI 
- `NAMEatomwise_Info_distance_heavy_atoms.svg` — AMI vs. atom pair distance plot for heavy atoms  

(Here `NAME` represents the dipeptide code, e.g., ALAALA.)

## Citation
If you use this dataset in your work, please cite:
https://doi.org/10.26434/chemrxiv-2024-2qs86
