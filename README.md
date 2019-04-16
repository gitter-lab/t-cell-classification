# T-cell classification
[![Build Status](https://travis-ci.com/gitter-lab/t-cell-classification.svg?branch=master)](https://travis-ci.com/gitter-lab/t-cell-classification)
[![Build status](https://ci.appveyor.com/api/projects/status/4nn776bdps5880h6/branch/master?svg=true)](https://ci.appveyor.com/project/gitter-lab/t-cell-classification/branch/master)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.2640835.svg)](https://doi.org/10.5281/zenodo.2640835)

This repository contains code for a work-in-progress manuscript on T-cell classification.

## Description

|Directory/File|Renderer|Description|
|:---|:---|:---|
|[images](./images)||Directory containing T-cell images|
|[plots](./plots)||Directory containing supplementary figures|
|[resource](./resource)||Directory containing supplementary training files|
|[image_processing.ipynb](./image_processing.ipynb) |<a href="https://nbviewer.jupyter.org/github/gitter-lab/t-cell-classification/blob/master/image_processing.ipynb"><img src="./plots/nbviewer_logo.png" height="16" align="bottom"></a>|Notebook for image cropping, filtering and mask measurement|
|[frequency_classifier.ipynb](./frequency_classifier.ipynb)|<a href="https://nbviewer.jupyter.org/github/gitter-lab/t-cell-classification/blob/master/frequency_classifier.ipynb"><img src="./plots/nbviewer_logo.png" height="16" align="bottom"></a>|Notebook for a trivial frequency classifier|
|[logistic_regression.ipynb](./logistic_regression.ipynb)|<a href="https://nbviewer.jupyter.org/github/gitter-lab/t-cell-classification/blob/master/logistic_regression.ipynb"><img src="./plots/nbviewer_logo.png" height="16" align="bottom"></a>|Notebook for fitting three logistic regression models with different feature vectors|
|[simple_neural_network.ipynb](./simple_neural_network.ipynb)|<a href="https://nbviewer.jupyter.org/github/gitter-lab/t-cell-classification/blob/master/simple_neural_network.ipynb"><img src="./plots/nbviewer_logo.png" height="16" align="bottom"></a>|Notebook for training a one-layer fully connected neural network|
|[simple_cnn_lenet.ipynb](./simple_cnn_lenet.ipynb)|<a href="https://nbviewer.jupyter.org/github/gitter-lab/t-cell-classification/blob/master/simple_cnn_lenet.ipynb"><img src="./plots/nbviewer_logo.png" height="16" align="bottom"></a>|Notebook for end-to-end training CNN LeNet|
|[transfer_learning.ipynb](./transfer_learning.ipynb)|<a href="https://nbviewer.jupyter.org/github/gitter-lab/t-cell-classification/blob/master/transfer_learning.ipynb"><img src="./plots/nbviewer_logo.png" height="16" align="bottom"></a>|Notebook for retraining layers of pre-trained Inception v3|

## License
The software is available under the MIT license.

## Citation
Pre-print by Zijie Wang, Alex J. Walsh, Melissa C. Skala, and Anthony Gitter coming soon.

## Acknowledgements
