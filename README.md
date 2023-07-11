# Line melting and the `obplib` library
Line melting is the most common melting pattern for Electron Beam Manufacturing due to its simplicity and effectiveness. Freemelt has developed the open source Python library `obplib` in order to facilitate line melting development and increase productivity. 

## Code Examples 
There are four examples, providing a step-by-step introduction to `obplib` by gradually increasing complexity:

1. A look at the library and its fundamental object, the humble `Point`. From there, `Line` objects and a first look at the `.obp` file format. 
2. Building a honeycomb pattern from scratch using a class and a grid of points. [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/olofficial/hex-test/main?labpath=honeycomb.ipynb)
3. Implementation of island melting: Partitioning the build area into a grid of overlapping islands, melting each of these separately in a certain order. This allows for a larger build area than ordinary line melting.
4. A look at some of the more advanced functionalities: curves, accelerating lines, timed points and transformations.

It is recommended that these are worked through in order, as at least the honeycomb and island melting Notebooks build upon the previous one.

# Jupyter Notebooks
Jupyter Notebooks are a useful tool for developing and sharing code in an interactive way. 
They are made up of cells organized in a linear order. There are two kinds of cells, code cells and text cells.
### Code cells
  Code cells allow the user to write and execute code. They can be run by pressing the "run" button or by clicking on them and using the keyboard shortcut CTRL+Enter. The output of the code cell is displayed below it.

### Text cells
Text cells are written in Markdown and contain information for the user about the code, and the problem it tries to solve.

More information can be found in the [Jupyter Notebook documentation](https://jupyter-notebook.readthedocs.io/).

# Running the Notebooks
Every notebook is hosted on MyBinder, allowing for learning without having a code editor installed on the computer. They are accessed by clicking the links in the [Code Examples](#code-examples) list. The notebooks are run remotely in a Docker container, and the launch time can be up to a minute long depending on conditions. 

## Saving and exporting
The MyBinder container is *stateless*, meaning that it doesn't save modifications made during the session. To retain these, the user can download the Notebook in the `.ipynb` format. Many code editors, such as VS Code, have native support for Jupyter notebooks. 
The notebooks can also be exported to formats including PDF, HTML and Markdown, allowing for easy sharing with non-Jupyter users. 

