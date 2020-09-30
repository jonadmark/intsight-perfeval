# IntSight Performance Evaluation

Jupyter notebook and scripts for the performance evaluation of the IntSight Paper.

## Environment Setup

Use the command bellow to clone this repository along with all its submodules:

```
git clone --recurse-submodules https://github.com/jonadmark/intsight-perfeval.git
```

The main files in this repository are `repetita2json.py` and `performance-evaluation.ipynb`. The first, `repetita2json.py`, depends on Python3 to be run and the `Repetita` submodule, which contains the networks from the TopologyZoo and RocketFuel projects. The `performance-evaluation.ipynb` notebook has the following Python3 libraries as dependencies:
- [Jupyter Notebooks](https://jupyter.org/install)
- [NetworkX](https://networkx.github.io/documentation/stable/install.html) for Python3
- [NumPy](https://numpy.org/install/)
- [Pandas](https://pandas.pydata.org/getting_started.html)
- [MatPlotLib](https://matplotlib.org/users/installing.html)

Note: We recommend installing all Python dependencies using the [Conda](https://docs.conda.io/en/latest/miniconda.html) package, dependency and environment management tool.

## Running the Performance Evaluation

With all the dependencies installed and the Repetitate submodule loaded, run the following command:

```
python3 repetita2json.py
```

This script converts Repetita topology and demand textual descriptions into json files that are readily readable by the `performance-evaluation.ipynb` notebook, which can be opened with the following command:

```
jupyter notebook performance-evaluation.ipynb
```

This notebook implements the analytical modelling for performance comparison between monitoring approaches and generates the figures available in the `paper_results` directory.
