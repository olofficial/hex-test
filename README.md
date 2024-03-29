# Line Melting and the `obplib` Library <img align="right" width="192" height="64" src="https://freemelt.com/app/uploads/freemeltLogo-1.png">

Line melting is a widely used melting pattern in Electron Beam Manufacturing due to its simplicity and effectiveness. To streamline line melting development and enhance productivity, Freemelt has created the open-source Python library `obplib`.

## Code Examples

The `obplib` library offers five code tutorials that provide a gradual introduction to its functionalities, increasing in complexity:

1. Library Overview: Introduction to the library and its fundamental object, the `Point`. It also covers `Line` objects and provides an initial look at the `.obp` file format. [![Launch Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/olofficial/hex-test/main?labpath=introduction.ipynb)

2. Cube grid: Creating an `.obp` build file of 3$`\times`$3 cubes using a class and a grid of points. This guide is for the user who wants to get started quickly by providing a build file creation template. [![Launch Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/olofficial/hex-test/main?labpath=cubes.ipynb)

3. Honeycomb Pattern: Step-by-step creation of a honeycomb pattern from scratch. [![Launch Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/olofficial/hex-test/main?labpath=honeycomb.ipynb)

4. Island Melting: Implementation of island melting by partitioning the build area into a grid of overlapping islands and melting them separately in a specific order. This technique enables a larger build area compared to ordinary line melting. [![Launch Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/olofficial/hex-test/main?labpath=islands.ipynb)

5. Curves: An introduction to Bézier curves and their implementation in `obplib`, a unique capability for Freemelt's machines. [![Launch Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/olofficial/hex-test/main?labpath=curves.ipynb)

6. Accelerating `Line` and `Curve` objects and their implementation. [![Launch Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/olofficial/hex-test/main?labpath=acceleration.ipynb)

7. Timed Points (spot melting). [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/olofficial/hex-test/main?labpath=timed_points.ipynb)

8. Transformations of `obplib` objects such as rotation, translation and scaling. [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/olofficial/hex-test/main?labpath=transformations.ipynb)

It is recommended to follow these examples in order, as many notebooks build upon concepts introduced in previous examples.

# Jupyter Notebooks

Jupyter Notebooks are valuable tools for interactive code development and sharing. They consist of cells organized in a linear order, with two primary cell types: code cells and text cells.

**Code cells** allow users to write and execute code. They can be run by clicking the "Run" button or by using the keyboard shortcut CTRL+Enter. The output of a code cell is displayed below it.

**Text cells** are written in Markdown and provide information and explanations about the code and the problem it addresses.

For further details, consult the [Jupyter Notebook documentation](https://jupyter-notebook.readthedocs.io/).

# Running the Notebooks

All the notebooks are hosted on MyBinder, enabling learning without requiring a local code editor installation. To access the notebooks, simply click the links provided in the [Code Examples](#code-examples) section. The notebooks run remotely in a Docker container, and the launch time may take up to a minute depending on conditions. If either the dependencies of the notebooks, or the notebooks themselves, are updated then the launch time rises to several minutes.

## Viewers

`obplib` includes its own line viewer called `obpviewer`, which allows for step-by-step visualization of line melting. However, since servers lack graphical interfaces, using `obpviewer` within MyBinder is not feasible. To overcome this limitation, a lightweight alternative called `notebook_viewer` has been developed. When running the notebook on your computer, you have the option to choose between these two viewers.

For optimal functionality and speed, it is recommended to use `obpviewer` on your computer. To enable this, save the `.obp` file and run `obpviewer [FILE PATH]/FILENAME.obp` in a command line interpreter. This allows the notebook to leverage the enhanced features and better performance provided by `obpviewer`.

## Saving and Exporting

The MyBinder container is *stateless*, meaning that it does not save modifications made during the session. To retain your changes, you can download the notebook in the `.ipynb` format. Many code editors, such as VS Code, have native support for Jupyter notebooks.

Additionally, the notebooks can be exported to formats like PDF, HTML, and Markdown, enabling easy sharing with non-Jupyter users.
