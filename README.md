# Pigs counting

This repo is a official implementation of ["Towards perspective-free object counting with deep learning"](http://agamenon.tsc.uah.es/Investigacion/gram/publications/eccv2016-onoro.pdf) on object counting with deep learning based on gramuah's code [CCNN](https://github.com/gramuah/ccnn).
Many thanks to  Daniel Oñoro-Rubio and Roberto J. López-Sastre for their codes.

## Introduction

Based on this code, it is improved to make it more suitable for pig counts.
We have provided the test code, you can test it directly, and all the code will be published after the article is published

## Citing Counting CNN

```
@inproceedings{onoro2016,
    Author = {O\~noro-Rubio, D. and L\'opez-Sastre, R.~J.},
    Title = {Towards perspective-free object counting with deep learning},
    Booktitle = {ECCV},
    Year = {2016}
}
```

## License
The license information of this project is described in the file "LICENSE.txt".

## Contents
1. [Requirements: software](#requirements-software)
2. [Requirements: hardware](#requirements-hardware)
3. [Basic installation](#basic-installation-sufficient-for-the-demo)
4. [Demo](#demo)
5. [How to reproduce the results of the paper](#how-to-reproduce-the-results-of-the-paper)
6. [Remarks](#remarks)
7. [Acknowledgements](#acknowledgements)

### Requirements: software

1. Use a Linux distribution. We have developed and tested the code on [Ubuntu](http://www.ubuntu.com/).


2. Requirements for `Caffe` and `pycaffe`. Follow the [Caffe installation instructions](http://caffe.berkeleyvision.org/installation.html).

  **Note:** Caffe *must* be built with support for Python layers!

  ```make
  # In your Makefile.config, make sure to have this line uncommented
  WITH_PYTHON_LAYER := 1
  ```

3. Python packages you need: `cython`, `python-opencv`, `python-h5py`, `easydict`, `pillow (version >= 3.4.2)`.


### Requirements: hardware

This code allows the usage of CPU and GPU, but we strongly recommend the usage of GPU.

1. For training, we recommend using a GPU with at least 3GB of memory.

2. For testing, a GPU with 2GB of memory is enough.

### Basic installation (sufficient for the demo)

1. Be sure you have added to your `PATH` the `tools` directory of your `Caffe` installation:

    ```Shell
    export PATH=<your_caffe_root_path>/build/tools:$PATH
    ```
    
2. Be sure you have added your `pycaffe` compilation into your `PYTHONPATH`:
    
    ```Shell
    export PYTHONPATH=<your_caffe_root_path>/python:$PYTHONPATH
    ```
    
