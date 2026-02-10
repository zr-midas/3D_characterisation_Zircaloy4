<br />
<p align="center">

  <h1 align="center">3D characterisation Zircaloy4</h1>

  <p align="center">
    This repository contains scripts and Dream3d pipelines for the reconstruction and analysis of 3D-EBSD data
    <br />
    <a href="https://github.com/zr-midas/3D_characterisation_Zircaloy4">Explore the docs</a>
    .
    <a href="https://github.com/zr-midas/3D_characterisation_Zircaloy4/blob/main/README.md">Read Documentation</a>
    ·
    <a href="https://github.com/zr-midas/3D_characterisation_Zircaloy4/issues">Report Bug</a>
    .
    <a href="https://github.com/zr-midas/3D_characterisation_Zircaloy4/blob/main/LICENSE">License</a>
  </p>
</p>


<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of contents:</summary>
  <ol>
    <li><a href="#about-the-project">About the project</a></li>
    <li>
      <a href="#getting-started">Getting started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li>
      <a href="#3d-characterisation-tools">3D characterisation tools</a></li>
      <ul>
        <li><a href="#3d-ebsd-reconstruction">3D EBSD reconstruction</a></li>
        <li><a href="#basal-gb-angles">Basal GB angles</a></li>
        <li><a href="#csl-analysis">CSL analysis</a></li>
        <li><a href="#kam-analysis">KAM analysis</a></li>
        <li><a href="#c-axis-misorientation">c-axis misorientation</a></li>
      </ul>
    </li>
    <li><a href="#acknowledgements">Acknowledgements</a></li>
  </ol>
</details>

## About the project

This repository supports the methodology described in the paper (doi_link) about characterising hydrides in Zircaloy 4 using 3D-EBSD data and advanced [3D characterisation](https://github.com/zr-midas/3D_characterisation_Zircaloy4/tree/main/3D_charaterisation) tools. 

## Getting started

This project uses [Poetry](https://python-poetry.org/) for dependency management. All required libraries and their versions are defined in the pyproject.toml file. Poetry can be installed with pip. Further instructions can be found in the [Poetry documentation](https://python-poetry.org/docs/).


### Prerequisites: 

Poetry installation
  ```sh
   pip install poetry
   ```

### Installation:

  1. **Clone the reposiroty**
   ```sh
   git clone https://github.com/zr-midas/3D_characterisation_Zircaloy4.git
   ```
   
  2. **Install dependencies**
   
Poetry will automatically create and activate a virtual environment where all required dependencies listed in pyproject.toml are installed.
   ```sh
   poetry install
   ```

  3. **Run the scripts**

   ```sh
   poetry run jupyter notebook
   ```
   
**Notes:**

Do not install dependencies manually with pip. Use always poetry install.

If you encounter dependency issues, try:

   ```sh
   poetry update
   ```
To see all installed packages run:
   ```sh
   poetry show
   ```

## [3D characterisation](https://github.com/zr-midas/3D_characterisation_Zircaloy4/tree/main/3D_charaterisation) tools

### [3D EBSD reconstruction](https://github.com/zr-midas/3D_characterisation_Zircaloy4/tree/main/3D_charaterisation/3D_EBSD_reconstruction)

This folder contains...

### [Basal GB angles](https://github.com/zr-midas/3D_characterisation_Zircaloy4/tree/main/3D_charaterisation/Basal_GB_angles)

The angle between the basal plane and the grain boundary plane wass calculated for the grains forming OR with the hydrides

### [CSL analysis](https://github.com/zr-midas/3D_characterisation_Zircaloy4/tree/main/3D_charaterisation/CSL_analysis)

The coincident site lattice (CSL) analysis was used to identify the boundaries between different variants in the hydrides.

<img width="466" height="197" alt="image" src="https://github.com/user-attachments/assets/7700fe1b-d45e-44ec-b0d1-cdbf5663bc7a" />


### [KAM analysis](https://github.com/zr-midas/3D_characterisation_Zircaloy4/tree/main/3D_charaterisation/KAM_analysis)

The kernel average misorientation (KAM) is a measure of local crystallographic misorientation and can be used to identify local misorientaions in the Zr grains or hydrides.

<img width="324" height="389" alt="image" src="https://github.com/user-attachments/assets/2a3cbec9-5180-4787-a521-5c399466d804" />

### [c-axis misorientation](https://github.com/zr-midas/3D_characterisation_Zircaloy4/tree/main/3D_charaterisation/c-axis_misorientation)

## Acknowledgements
* [MIDAS](https://www.zr-midas.org/)
* [MTex](https://mtex-toolbox.github.io/)
* [Dream.3D](https://www.dream3d.io/blog/)
* [PyVista](https://docs.pyvista.org/)
* [Numpy](https://numpy.org/)
* [Matplotlib](https://matplotlib.org/)
* [h5py](https://www.h5py.org/)
* [Pandas](https://pandas.pydata.org/)
* [Scipy](https://scipy.org/)
