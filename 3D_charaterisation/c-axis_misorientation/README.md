# c-axis misorientation

This folder has the methodology for finding the angles between pairs of grains with hydrides at their interface, and it contains:

- A Dream.3D pipeline that calculates the c-axis misorientation between adjacent grains. 

- A Jupyter notebook that exports a csv file with all the angles sorted in a list for easier identification of the angles of the pair of grains of interest in Paraview.

- A Jupyter notebook that plots the graph comparing the resulting angles with ranges of values that were reported in the literature.


## Input files:

- Dream3D file with the reconstructed 3D-EBSD data.

## Exported files:

- Dream3D file with the angles of c-axis misalignment.

- Xdmf file that can be opened with Paraview to visualise the data saved in the Dream3D file for each voxel of the 3D microstructure.

- CSV file with the list of grain ID, the grain ID of all their neighbouring grains, and the c-axis misalignment angle between each couple of grains:

  <img width="214" height="221" alt="image" src="https://github.com/user-attachments/assets/e1e28d8e-4abf-4071-9eeb-603889f44ddf" />

  In [Paraview](https://www.paraview.org/), the grain IDs of grains with hydrides at their interfaces can be identified, and their corresponding c-axis misalignments can be checked in the list of this csv file.
