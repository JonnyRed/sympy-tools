
# Sympy-tools

Sympy-tools is a collection of useful tools and utilities for Sympy,
a Python library for symbolic mathematics.

# Installation

* miniconda distribution installed  on your system.
* This installation is based on the very nicely explained
by [Bits of Analytics][] in the document [Using pip with conda][] for local development projects document.
* The installation will be installed into a conda environment.
  * The env will  be named `sympy_tools` (you can change this).

The `sympy_tools` environment will be installed thus:

```miniconda
<user directory>\sympy\sympy-tools>conda env create -f "D:\Users\John\Documents\IPython Notebooks\sympy\sympy-tools\environment.yml"
```

* `<user directory>\sympy\sympy-tools>` is the directory where you want to install `sympy-tools`
* `environment.yml` is the conda yml environment to create.
  * `pip` is the last utility to be installed
* For the `sympy-tools` environment
* If the environment is to be changed then a complete  new conda environment should be  be created.

```yml
name: sympytools
channels:
  - conda-forge
  - bokeh
  - defaults
dependencies:
  - python=3.10
  - ipython
  - ipykernel
  - numpy
  - matplotlib
  - seaborn
  - pandas
  - sympy
  - scipy
  - statsmodels
  - notebook
  - adaptive
  - panel
  - ipywidgets
  - ipympl
  - ipywidgets_bokeh
  - colorcet
  - k3d
  - msgpack-python
  - plotly::plotly
  - vtk
  - sympy_plot_backends
  - pip
prefix: D:\Users\John\miniconda3\envs\sympytools
```

To install `Sympy-tools` in the environment

* pip  must be from the conda environment
* The pip command must be executed in the `sympytools` source directory.
  * `pip install -e .` ensures that  any changes made to the package are immediately available.

```miniconda
\Users\John\Documents\IPython Notebooks\sympy\sympy-tools>D:\Users\John\miniconda3\envs\sympytools\Scripts\pip install -e .
 ```

A minimalist `setup` script is provided.

# Usage

TODO provide example

[Bits of Analytics]:https://bitsofanalytics.org/

[Using pip with conda]:https://bitsofanalytics.org/posts/pip-conda-local-dev/pip_conda_local_dev.html

# Testing

TODO add doctests that exist in the code already

# License

Sympy-tools is released under the MIT License.

# Acknowledgments

Sympy-tools would not be possible without the Sympy library.

Please note that this is a basic template, and you should customize it to
fit the specifics of your package. For example, you might want to include
more detailed usage examples, information about the package's architecture,
or a roadmap for future development
