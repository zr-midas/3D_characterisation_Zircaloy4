# 3D-EBSD reconstruction 

This repository contains the pipelines to process 3D-EBSD Zr microstructures:

0– Import_ctfs pipeline imports the EBSD maps acquired from each slice of the 3D-EBSD experiment and combines them into a single file containing all the data.

1- Rotations pipeline applies the necessary rotation of the crystal orientations so the euler space matches the sample reference frame.

2- Alignment pipeline contains the alignment method for the studied 3D microstructures. Alignment based on a misorientation threshold of 5 was used.

3- Cleaning pipeline was used to remove voxels in blank and noise in Zr phase (isolated voxels across the microstructure). The isolated hydride voxels were not removed, as they are more likely associated with poor hydride indexing rather than noise, and their removal could interfere with the quantitative analysis of hydrides.

## Requirements:

EBSD maps with the format .ctf

## Files exported:

Hierarquical files with extension .dream3d that can be access with tools like HDFview software or in python with:

```
import h5py

file_path = 'path/to/the/dream3d/file'
file_name = file_path + 'path/to/the/file.dream3d'

data_of_interest = "DataContainers/CellData/data_of_interest" # Search the correct path in your file

with h5py.File(fine_name, "r"):
    variable_with_data_of_interest = f[data_of_interest][()]

```


These pipelines also export .xdmf files that can be opened in Paraview to visualise the reconstructed microstructures in 3D.
