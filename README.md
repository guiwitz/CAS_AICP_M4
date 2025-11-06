[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/guiwitz/CAS_AICP_M4/blob/main)

# Image module for AICP CAS at DSL

This repository contains the notebooks and scripts for the Image module of the **A**rticifial **I**ntelligence in **C**reative **P**ractices CAS at DSL.

## Installation
To use the repository, either clone it using git, download it as a zip file (green button on the top right) or download individual files using the Download button on the top right of the file view. To run the notebooks, make sure you have the ```data``` folder placed in the same directory as the notebooks.

To install required packages we recommend using conda to manage environments. Different parts of the course have different requirements and some notebooks are meant to rather run on Google Colab for GPU access. For the initial introduction to image handling in Python, you can use the following environment, which should install relatively quickly:

```bash
conda create -n aicp_image python=3.12 jupyterlab numpy matplotlib scikit-image ghostscript pillow -c conda-forge
```

Alternatively, you can create the following full environment that will give you access to certain deep learning models like YOLO and replicate API etc.: 

```bash
conda create -n aicp_image_full python=3.12 jupyterlab numpy matplotlib scikit-image ghostscript pytorch torchvision pillow replicate ultralytics -c conda-forge
```

To use the environments, activate them using their name e.g.:

```bash
conda activate aicp_image
```

To start Jupyter Lab, run:

```bash
jupyter lab
```