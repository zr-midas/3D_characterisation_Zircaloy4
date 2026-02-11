# CSL analysis

This repository contains a Dream.3D pipeline to identify the CSL boundaries in the hydrides phase. 

## Input files:

Dream3D file with the reconstructed 3D-EBSD data.

## Exported files:

- Dream3d file that can be opened with HDFview or h5py package in Python.
- The corresponding xdmf file for 3D visualisation in Paraview:

<img width="352" height="255" alt="image" src="https://github.com/user-attachments/assets/beff9734-6d9b-4d4a-8a81-e610128383d5" />

Important: The XDMF files do not storage data, only the dream3d files do. The XDMF file must be located in the same folder as the corresponding dream3d file so that ParaView can correctly read the data from dream3d file when the XDMF file is opened.
