[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/guiwitz/CAS_AICP_M4/blob/main)

# Image module for AICP CAS at DSL

This repository contains the notebooks and scripts for the Image module of the **A**rticifial **I**ntelligence in **C**reative **P**ractices CAS at DSL.

## Installation
To use the repository, either clone it using git, download it as a zip file (green button on the top right) or download individual files using the Download button on the top right of the file view. To run the notebooks, make sure you have the ```data``` folder placed in the same directory as the notebooks.

To install required packages we recommend using conda to manage environments. Different parts of the course have different requirements and some notebooks are meant to rather run on Google Colab for GPU access. For the initial introduction to image handling in Python, you can use the following environment, which should install relatively quickly:

```bash
conda create -n aicp_image python=3.14 jupyterlab numpy matplotlib scikit-image pillow openai napari pyqt6 -c conda-forge
```

Alternatively, you can create the following full environment that will give you access to certain deep learning models like YOLO and replicate API etc.: 

```bash
conda create -n aicp_image_full python=3.14 jupyterlab numpy matplotlib scikit-image openai napari pyqt6 pytorch torchvision pillow replicate ultralytics -c conda-forge
```

To use the environments, activate them using their name e.g.:

```bash
conda activate aicp_image
```

## Interactive computing

You can run notebooks either in Jupyter Lab or in VSCode using the appropriate kernel.

To start Jupyter Lab, run:

```bash
jupyter lab
```

To use the environment in VSCode, open a notebook, and select in the top right the kernel corresponding to the environment you created (e.g., `aicp_image` or `aicp_image_full`).

## Using uv

uv is an alternative package manager. If you are using it, go to the repository folder and create a virtual environment there:

```bash
uv venv --python 3.14
```

Then install the packages for the basic environment:

```bash
uv pip install jupyterlab numpy matplotlib scikit-image pillow openai "napari[pyqt6]"
```

For the advanced environment, additionally install:

```bash
uv pip install torch torchvision replicate ultralytics
```

uv creates the environment in a `.venv` folder inside the repository. To start Jupyter Lab, run:

```bash
uv run jupyter lab
```

In VSCode, select the `.venv` kernel in the top right of the notebook. 