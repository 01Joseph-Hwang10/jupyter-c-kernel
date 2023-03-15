# Jupyter C Kernel

This project was originally forked from <https://github.com/brendan-rius/jupyter-c-kernel>.

The main purpose of this project is to let myself allow to notetake CSE lectures with relevant code that can be executed in the notebook. So it might not be suitable for the people who demands a full-featured C kernel for production.

It includes a few improvements:

**You can include another c file in your workspace with the `#include` directive.** 

Example code is provided in the `examples` folder. Keep in mind that c file and header file should be in a same level of directory. In other words, it's not allowed to have a header file in include directory and c file in src directory. Instead, you should have both in the same directory.

**Minor refactoring**

There were some minor refactoring in both c and python code.

# Origianl README

Check out the original README for further details: <https://github.com/XaverKlemenschits/jupyter-c-kernel#readme>
