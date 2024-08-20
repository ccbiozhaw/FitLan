## This is the GitHub Repository for the publication: 

# Enriching productive mutational paths accelerates enzyme evolution (https://doi.org/10.1038/s41589-024-01712-3)

In this repository we provide both data and code that were used to calculate ddG values with PyRosetta, as well as to visualize the fitness landscape of shuffle-library variants.

## System requirements
All software dependencies are defined via the anaconda yml files or can installed utilizing the requirements.txt files.
We expect that the code works on all opeating systems that support anaconda or miniconda 3. However, we have only tested the software using Ubuntu 22.04.
No special hardware is needed, however the prinicipal component analysis needed as prerequisite for the fitness landscape plotting might profit from GPU computation (e.g. using NVIDIA GPUs with CUDA).

## Installation guide
We recommend to install the needed dependencies for both the fitness landscape and the ddG calculation utilizing the provided anaconda yml files:
conda env create -f environment.yml
In rare cases, it might be necessary to install missing or incompatible instances via pip. 
You can also install the requirements via "pip install -r requirements.txt".
The typical installation time should take less than 5 minutes.

As we use PyRosetta, a valid Rosetta license is needed to run the ddG determination.

## Demo
Exemplary input files and expected outputs can be found in the respective folder for the fitness landscape and the ddG calculation.
Despite of the principal component analysis (which takes <1 h on our server), the run should finish in less than 10 minutes on a "normal" desktop computer.
However, we provide the output of the principal component analysis. Thus, the second script of the fitness landscape plotting can be performed even if the first script takes to long. 

## Instructions for use
After installation of all dependencies, activate the conda environment if needed and start a jupyter notebook server.

For calculation of ddG values, first start the relax.ipynb notebook and execute all cells to relax your input protein structure. 
Secondly, you can execute the ddg.ipynb notebook to calculate the ddG scores of all amino acid substitutions.

To enable fitness landscape plotting, you first have to generate ESM-2 embeddings and run the principal component analysis using make_embeddings.ipynb to generate the encoding of all variants.
Afterwards, you can plot the fitness landscape as 3D surface using plot_3d_surface.ipynb.

# References
This code originates from the following publication:

https://doi.org/10.1038/s41589-024-01712-3

If you utilize this code, please cite:

https://doi.org/10.1038/s41589-024-01712-3

https://doi.org/10.1016/j.csbj.2023.09.013
