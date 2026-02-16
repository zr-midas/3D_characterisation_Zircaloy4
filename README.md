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
    <a href="https://github.com/zr-midas/3D_characterisation_Zircaloy4/issues">Report errors</a>
    .
    <a href="https://github.com/zr-midas/3D_characterisation_Zircaloy4/blob/main/LICENSE">License</a>
  </p>
</p>



https://github.com/user-attachments/assets/31c36508-1feb-49e1-acc4-b650f364d373



<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of contents:</summary>
  <ol>
    <li><a href="#about-the-project">About the project</a></li>
    <li><a href="#prerequisites">Prerequisites</a></li>
    <li><a href="#getting-started">Getting started</a></li>
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

This repository supports the methodology described in the paper (doi_link) for characterising hydrides in Zircaloy-4 using 3D-EBSD data and advanced [3D characterisation](https://github.com/zr-midas/3D_characterisation_Zircaloy4/tree/main/3D_charaterisation) tools. 

## Prerequisites

This repository contain Dream.3D pipelines that can be open with Dream.3D software and Jupyter Notebook scripts to be run with Python: 

- Dream.3D version 6 --> https://dream3d.bluequartz.net/Download/
- Python >=3.13 (version requirement in `pyproject.toml`)
  
>### Poetry installation:

This project uses [Poetry](https://python-poetry.org/) for dependency management. All required libraries and their versions are defined in the pyproject.toml file. Poetry can be installed with pip. Further instructions can be found in the [Poetry documentation](https://python-poetry.org/docs/).

  ```sh
   pip install poetry
   ```

## Getting started

  1. **Clone the repository**
     
   ```sh
   git clone https://github.com/zr-midas/3D_characterisation_Zircaloy4.git
   ```
   
  2. **Install dependencies**
   
> Option A: Poetry will automatically create and activate a virtual environment where all required dependencies listed in pyproject.toml are installed.

   ```sh
   poetry install
   ```
If you have more than one version of python, run:

   ```sh
    poetry env use python3.13
    poetry install
   ```

> Option B: Or you can install the dependencies with pip:

  ```sh
  pip install -r requirements.txt
  ```

  3. **Run the scripts**

   ```sh
   poetry run jupyter notebook
   ```
   

## [3D characterisation](https://github.com/zr-midas/3D_characterisation_Zircaloy4/tree/main/3D_charaterisation) tools

This folder contains all the workflows developed for the 3D reconstruction and analysis of 3D-EBSD data:

### [3D EBSD reconstruction](https://github.com/zr-midas/3D_characterisation_Zircaloy4/tree/main/3D_charaterisation/3D_EBSD_reconstruction)

This project uses [Dream.3D](https://www.dream3d.io/) to perform 3D reconstruction of 3D-EBSD data and obtain 3D microstructures that display the 3D morphology of alpha-Zr grains and hydrides. 
The Dream.3D pipelines developed for the 3D reconstruction can be found in this folder. 

<img width="621" height="430" alt="image" src="https://github.com/user-attachments/assets/fa15578d-22ae-410e-8f45-5063f8300900" />


### [Basal GB angles](https://github.com/zr-midas/3D_characterisation_Zircaloy4/tree/main/3D_charaterisation/Basal_GB_angles)

The angle between the basal plane and the grain boundary plane was calculated for grains forming an orientation relationship (OR) with hydrides. Previous studies have reported that these angles fall within specific ranges when a hydride precipitated at the grain boundary. Investigating the relationship between these angles and preferential hydride precipitation could improve our understanding of hydride precipitation in Zr alloys.

<img width="320" height="294" alt="image" src="https://github.com/user-attachments/assets/c18db9c2-c63a-4c6f-a06a-bbe1697c6f7e" />

### [CSL analysis](https://github.com/zr-midas/3D_characterisation_Zircaloy4/tree/main/3D_charaterisation/CSL_analysis)

The coincident site lattice (CSL) analysis was used to identify the boundaries between different variants in the hydrides.

<img width="466" height="197" alt="image" src="https://github.com/user-attachments/assets/7700fe1b-d45e-44ec-b0d1-cdbf5663bc7a" />

### [KAM analysis](https://github.com/zr-midas/3D_characterisation_Zircaloy4/tree/main/3D_charaterisation/KAM_analysis)

The kernel average misorientation (KAM) is a measure of local crystallographic misorientation and can be used to identify local misorientaions in the Zr grains or hydrides.

<img width="324" height="389" alt="image" src="https://github.com/user-attachments/assets/2a3cbec9-5180-4787-a521-5c399466d804" />

### [c-axis misorientation](https://github.com/zr-midas/3D_characterisation_Zircaloy4/tree/main/3D_charaterisation/c-axis_misorientation)

The misalignment between the c-axis of crystal orientation of two adjacent grains was calculated with Dream.3D. As for basal-GB angles, previous studies have found that these angles tend to fall within specific ranges, and investigating these c-axis misorientations could also help with the understanding of preferential sites for hydride precipitation in Zr alloys.

<img width="756" height="224" alt="image" src="https://github.com/user-attachments/assets/acdd8af9-e804-45c6-8c1d-ceabd4a2c834" />

## Acknowledgements

The authors acknowledge funding from the Engineering and Physical Sciences Research Council UK for funding the study through the MIDAS (Mechanistic understanding of Irradiation Damage in fuel Assemblies) programme grant (EP/S01702X/1). Rolls-Royce plc and Amentum are acknowledged for the provision of materials and financial support. The authors acknowledge the Royce Institute for Advanced Materials, funded through EPSRC grants EP/R00661X/1, EP/S019367/1, EP/P025021/1 and EP/P025498/1 for supporting aspects of this research.

* [MIDAS](https://www.zr-midas.org/)
* [MTex](https://mtex-toolbox.github.io/)
* [Dream.3D](https://www.dream3d.io/blog/)
* [PyVista](https://docs.pyvista.org/)
* [Numpy](https://numpy.org/)
* [Matplotlib](https://matplotlib.org/)
* [h5py](https://www.h5py.org/)
* [Pandas](https://pandas.pydata.org/)
* [Scipy](https://scipy.org/)
