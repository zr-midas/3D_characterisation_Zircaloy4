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


Pending to add an interactive index here once all the folders are set up

## Installation and setup

This project uses [Poetry](https://python-poetry.org/) for dependency management. All required libraries and their versions are defined in the pyproject.toml file. Poetry can be installed with pip. Further instructions can be found in the [Poetry documentation](https://python-poetry.org/docs/).


1. **Poetry installation**
  ```sh
   pip install poetry
   ```

2. **Clone the reposiroty**
   ```sh
   git clone https://github.com/zr-midas/3D_characterisation_Zircaloy4.git
   ```
   
3. **Install dependencies**
   
Poetry will automatically create and activate a virtual environment where all required dependencies listed in pyproject.toml are installed:
   ```sh
   poetry install
   ```

4. **Run the scripts**

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

## Acknowledgements
* [MIDAS](https://www.zr-midas.org/)
* [MTex](https://mtex-toolbox.github.io/)
* [Dream.3D](https://www.dream3d.io/blog/)
* [PyVista](https://docs.pyvista.org/)
* [Numpy](https://numpy.org/)
* [Matplotlib](https://matplotlib.org/)
* [h5py](https://www.h5py.org/)
* [Pandas](https://pandas.pydata.org/)
