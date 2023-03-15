# Jupyter C Kernel

This project was originally forked from <https://github.com/brendan-rius/jupyter-c-kernel>.

The main purpose of this project is to let myself allow to notetake CSE lectures with relevant code that can be executed in the notebook. So it might not be suitable for the people who demands a full-featured C kernel for production.

It includes a few improvements:

**You can include another c file in your workspace with the `#include` directive.** 

Example code is provided in the `examples` folder. Keep in mind that c file and header file should be in a same level of directory. In other words, it's not allowed to have a header file in include directory and c file in src directory. Instead, you should have both in the same directory.

Also it is worth note that the absolute path of the file you want to include should only contain alphanumeric characters, and the following special characters: `.`, `-`, `_`, `/`.

**Minor refactoring**

There were some minor refactoring in both c and python code.

## Pre-requisites

1. gcc
2. Jupyter Notebook

## Installation

```bash
git clone https://github.com/01Joseph-Hwang10/jupyter-c-kernel
cd jupyter-c-kernel
pip install -r requirements.txt # Recommend to use virtualenv
cd jupyter_c_kernel
sudo python install_c_kernel
```

Make sure to reload the jupyter notebook after installation if there are existing running notebooks.

## Note

- This kernel was tested on:
  - M1 Macbook Air
  - OS: macOS Ventura 13.1
  - RAM: 16GB
  - gcc is provided by Xcode
- I did not tested the Dockerfile, so it might not work.

# Origianl README

Check out the original README for further details: <https://github.com/XaverKlemenschits/jupyter-c-kernel#readme>
