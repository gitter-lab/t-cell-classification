# T-cell classification
[![Build Status](https://travis-ci.com/gitter-lab/t-cell-classification.svg?branch=master)](https://travis-ci.com/gitter-lab/t-cell-classification)
[![Build status](https://ci.appveyor.com/api/projects/status/4nn776bdps5880h6/branch/master?svg=true)](https://ci.appveyor.com/project/gitter-lab/t-cell-classification/branch/master)
[![badge](./plots/binder_badge.svg)](https://mybinder.org/v2/gh/gitter-lab/t-cell-classification/master)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.2640835.svg)](https://doi.org/10.5281/zenodo.2640835)

This repository contains code for the manuscript **Classifying T cell activity in autofluorescence intensity images with convolutional neural networks**.

## Description

|Directory/File|Renderer|Description|
|:---|:---|:---|
|[images](./images)||Directory containing T-cell images|
|[plots](./plots)||Directory containing supplementary figures|
|[resource](./resource)||Directory containing supplementary training files|
|[image_processing.ipynb](./image_processing.ipynb) |<a href="https://nbviewer.jupyter.org/github/gitter-lab/t-cell-classification/blob/master/image_processing.ipynb"><img src="./plots/nbviewer_logo.png" height="16" align="bottom"></a> <a href="https://mybinder.org/v2/gh/gitter-lab/t-cell-classification/master?filepath=image_processing.ipynb"><img src="./plots/binder_logo.png" height="16" align="bottom"></a>|Notebook for image cropping, filtering and mask measurement|
|[frequency_classifier.ipynb](./frequency_classifier.ipynb)|<a href="https://nbviewer.jupyter.org/github/gitter-lab/t-cell-classification/blob/master/frequency_classifier.ipynb"><img src="./plots/nbviewer_logo.png" height="16" align="bottom"></a> <a href="https://mybinder.org/v2/gh/gitter-lab/t-cell-classification/master?filepath=frequency_classifier.ipynb"><img src="./plots/binder_logo.png" height="16" align="bottom"></a>|Notebook for a trivial frequency classifier|
|[logistic_regression.ipynb](./logistic_regression.ipynb)|<a href="https://nbviewer.jupyter.org/github/gitter-lab/t-cell-classification/blob/master/logistic_regression.ipynb"><img src="./plots/nbviewer_logo.png" height="16" align="bottom"></a> <a href="https://mybinder.org/v2/gh/gitter-lab/t-cell-classification/master?filepath=logistic_regression.ipynb"><img src="./plots/binder_logo.png" height="16" align="bottom"></a>|Notebook for fitting three logistic regression models with different feature vectors|
|[simple_neural_network.ipynb](./simple_neural_network.ipynb)|<a href="https://nbviewer.jupyter.org/github/gitter-lab/t-cell-classification/blob/master/simple_neural_network.ipynb"><img src="./plots/nbviewer_logo.png" height="16" align="bottom"></a> <a href="https://mybinder.org/v2/gh/gitter-lab/t-cell-classification/master?filepath=simple_neural_network.ipynb"><img src="./plots/binder_logo.png" height="16" align="bottom"></a>|Notebook for training a one-layer fully connected neural network|
|[simple_cnn_lenet.ipynb](./simple_cnn_lenet.ipynb)|<a href="https://nbviewer.jupyter.org/github/gitter-lab/t-cell-classification/blob/master/simple_cnn_lenet.ipynb"><img src="./plots/nbviewer_logo.png" height="16" align="bottom"></a> <a href="https://mybinder.org/v2/gh/gitter-lab/t-cell-classification/master?filepath=simple_cnn_lenet.ipynb"><img src="./plots/binder_logo.png" height="16" align="bottom"></a>|Notebook for end-to-end training CNN LeNet|
|[transfer_learning.ipynb](./transfer_learning.ipynb)|<a href="https://nbviewer.jupyter.org/github/gitter-lab/t-cell-classification/blob/master/transfer_learning.ipynb"><img src="./plots/nbviewer_logo.png" height="16" align="bottom"></a> <a href="https://mybinder.org/v2/gh/gitter-lab/t-cell-classification/master?filepath=transfer_learning.ipynb"><img src="./plots/binder_logo.png" height="16" align="bottom"></a>|Notebook for fine-tuning layers of pre-trained Inception v3|

<br/>

- [Nbviewer <img src="./plots/nbviewer_logo.png" height="16" align="bottom">](https://nbviewer.jupyter.org)  renders these notebooks as static HTML web pages.
- [Binder <img src="./plots/binder_logo.png" height="16" align="bottom">](https://mybinder.org) hosts an executable environment for notebooks.
- Three `conda` environment files are provided. `environment.yml` and `environment-windows.yml` include main dependencies with major versions for macOS/Linux and Windows respectively; `environment-complete.yml` provides a complete list of all packages and versions.
- You can use `conda env create -f {environment.yml|environment-windows.yml|environment-complete.yml}` to install dependencies. 

## License
The software is available under the BSD 3-Clause Clear License.

## Citation
Pre-print by Zijie J. Wang, Alex J. Walsh, Melissa C. Skala, and Anthony Gitter coming soon.