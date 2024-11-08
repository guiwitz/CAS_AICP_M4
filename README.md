[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/guiwitz/CAS_AICP_M4/blob/main)

# Image module for AICP CAS at DSL

This repository contains the notebooks and scripts for the Image module of the **A**rticifial **I**ntelligence in **C**reative **P**ractices CAS at DSL.

## Installation
To use the repository, either clone it using git, download it as a zip file (green button on the top right) or download individual files using the Download button on the top right of the file view. To run the notebooks, make sure you have the ```data``` folder placed in the same directory as the notebooks.

To install required packages we recommend using conda to manage environments. Different parts of the course have different requirements and some notebooks are meant to rather run on Google Colab for GPU access. You can create a minimal environment with the following command and further add packages as needed.

```bash
conda create -n aicp_image python=3.11 jupyterlab numpy matplotlib scikit-image ghostscript
```

To use the environment, activate it with:

```bash
conda activate aicp_image
```

To start Jupyter Lab, run:

```bash
jupyter lab
```