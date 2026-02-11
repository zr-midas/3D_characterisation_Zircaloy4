# KAM analysis

This repository contains:

- A Dream.3D pipeline that calculates the KAM at every voxel of the microstructure, using a kernel 3x3x3 (which corresponds to value 1 in the KAM filter)
- A Jupyter notebook that plots the graphs of KAM vs distance to hydride

## Input files:

- Dream3D file with the reconstructed 3D-EBSD data.

## Exported files:

- Dream3d file with the KAM values per voxel of the 3D microstructure, that can be read with the Jupyter notebook in this folder.
- The corresponding xdmf file for 3D visualisation in Paraview
- KAM vs distance to hydrides plots

<img width="324" height="389" alt="image" src="https://github.com/user-attachments/assets/2a3cbec9-5180-4787-a521-5c399466d804" />
