# Street View House Numbers
### Udacity Capstone by Daliso Zuze

## Files

SVHN_Image-Preprosessing.ipynb : 
- Downloads and preprocesses files used for training the Convolutional Nerural Network (CNN). It also includes code for generating the synthetic dataset.

SVHN_CNN-Implementation.ipynb  :
- Code for defining the CNN model and training the neural network.

SVHN_CNN-Predictions.ipynb : 
- Code for doing predictions on images using the model generated in the above implementation file.

## Installation

This project requires **Python 2.7** , IPython and libraries based on below import statements:

import tensorflow as tf

import prettytensor as pt

import numpy as np, h5py

import matplotlib.pyplot as plt

from matplotlib.font_manager import FontProperties

from PIL import Image, ImageDraw, ImageFont

from scipy import ndimage

from skimage.transform import resize

from __future__ import print_function

from IPython.display import display, Image

import sys

import os

import tarfile

import time

import gc

import random

from math import log

import logging

import time

from six.moves.urllib.request import urlretrieve

from six.moves import cPickle as pickle

from six.moves import range

from datetime import timedelta

from tqdm import tqdm, tnrange, tqdm_notebook

Note that suffient hard disk space will be required for storing the training and test datasets as well as the log files. It is recommended to use a machine with at least *20GB* of disk space available. Also sufficient RAM will be required to execute the IPython notebooks. It is recommended to use a machine with at least *15GB* of RAM available.

## Usage

Once everything is setup, simply execute the following files

SVHN_Image-Preprosessing.ipynb
- This will download data from http://ufldl.stanford.edu/housenumbers/ containing the Street View House Number dataset, generate a synthetic dataset, preprocess and package these in Pickle files for usage in the Implementation file.

SVHN_CNN-Implementation.ipynb
- This will load the preprocessed image files, train the neural network and periodically write results to a log file.

SVHN_CNN-Predictions.ipynb 
- This will load raw images from a specified folder (see configuration of the folder at beginning of notebook) and run predictions on them (these will be displayed at bottom). This has been design to ideally work with 9 images at a time.

