# 3D-EBSD reconstruction 

This repository contains the pipelines to process 3D-EBSD Zr microstructures

1-Rotations pipeline applies the necessary rotation of the crystal orientations so the euler space matches the sample reference frame

2- Alignment pipeline contains the alignment method for the studied 3D microstructures. Alignment based on a misorientation threshold of 5 was used.

3-Cleaning pipeline was used to remove voxels in blank and noise in Zr phase (isolated voxels across the microstructure). The isolated hydride voxels were not removed, as they are more likely associated with poor hydride indexing rather than noise, and their removal could interfere with the quantitative analysis of hydrides.

