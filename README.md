<img align="right" width="192" height="64" src="https://freemelt.com/app/uploads/freemeltLogo-1.png">

# Line Melting and the `obplib` Library

Line melting is a widely used melting pattern in Electron Beam Manufacturing due to its simplicity and effectiveness. To streamline line melting development and enhance productivity, Freemelt has created the open-source Python library called `obplib`.

## Code Examples

The `obplib` library offers five code tutorials that provide a gradual introduction to its functionalities, increasing in complexity:

1. Library Overview: Introduction to the library and its fundamental object, the `Point`. It also covers `Line` objects and provides an initial look at the `.obp` file format.[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/olofficial/hex-test/main?labpath=introduction.ipynb)
  
2. Cube grid: Creating an `.obp` build file of 3$`\times`$3 cubes using a class and a grid of points. [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/olofficial/hex-test/main?labpath=cubes.ipynb)
  
3. Honeycomb Pattern: Step-by-step creation of a honeycomb pattern from scratch. [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/olofficial/hex-test/main?labpath=honeycomb.ipynb)
   
4. Island Melting: Implementation of island melting by partitioning the build area into a grid of overlapping islands and melting them separately in a specific order. This technique enables a larger build area compared to ordinary line melting. [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/olofficial/hex-test/main?labpath=islands.ipynb)

5. Curves: An introduction to Bézier curves and their implementation in `obplib`. [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/olofficial/hex-test/07546d7c57a1fa6901cd5a2fdf428052cca51795?urlpath=lab%2Ftree%2Fcurves.ipynb)

6. Accelerating `Line` and `Curve` objects and their implementation.

7. Timed Points (point melting).

8. Transformations. 

It is recommended to follow these examples in order, as many notebooks build upon concepts introduced in previous examples.

# Jupyter Notebooks

Jupyter Notebooks are valuable tools for interactive code development and sharing. They consist of cells organized in a linear order, with two primary cell types: code cells and text cells.

**Code cells** allow users to write and execute code. They can be run by clicking the "Run" button or by using the keyboard shortcut CTRL+Enter. The output of a code cell is displayed below it.

**Text cells** are written in Markdown and provide information and explanations about the code and the problem it addresses.

For further details, consult the [Jupyter Notebook documentation](https://jupyter-notebook.readthedocs.io/).

# Running the Notebooks

All the notebooks are hosted on MyBinder, enabling learning without requiring a local code editor installation. To access the notebooks, simply click the links provided in the [Code Examples](#code-examples) section. The notebooks run remotely in a Docker container, and the launch time may take up to a minute depending on conditions.

## Viewers

`obplib` includes its own line viewer called `obpviewer`, which allows for step-by-step visualization of line melting. However, since servers typically lack graphical interfaces, using `obpviewer` within MyBinder is not feasible. To overcome this limitation, a lightweight alternative called `interactive_viewer` has been developed. When running the notebook on your computer, you have the option to choose between these two viewers.

For optimal functionality and speed, it is recommended to use `obpviewer` on your computer. To enable this, uncomment the relevant `obpviewer` lines and comment out the corresponding `interactive_viewer` lines in the code. This allows the notebook to leverage the enhanced features and faster performance provided by `obpviewer`.

## Saving and Exporting

The MyBinder container is *stateless*, meaning that it does not save modifications made during the session. To retain your changes, you can download the notebook in the `.ipynb` format. Many code editors, such as VS Code, have native support for Jupyter notebooks.

Additionally, the notebooks can be exported to formats like PDF, HTML, and Markdown, enabling easy sharing with non-Jupyter users.
