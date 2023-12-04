# LLE_Cupy

**Implementation of Graph Locally Linear Embedding (LLE) using Cupy**

This repository contains an accurate implementation of "Graph Locally Linear Embedding." The algorithm's details can be found in the paper ["Graph Embedding Techniques, Applications, and Performance: A Survey"](https://doi.org/10.1016/j.knosys.2018.03.022) by Palash Goyal and Emilio Ferrara (2018).

## Files

- **LLE_Cupy.py**: Contains the provided implementation of LLE.
  
- **Demonstration.ipynb**: A Jupyter notebook demonstrating our LLE implementation and highlighting the differences from the LLE implementation in the Python package nxt-gem. Ensure the following Python packages are also installed to run this notebook: matplotlib, sklearn, pyspark, networkx, nxt-gem.

- **evaluate_embedding.py**: Provides code for evaluating graph embeddings. This is also required to run **Demonstration.ipynb**.

## Requirements

Our implementation of "Locally Linear Embedding" relies on the [networkx](https://networkx.github.io/) package. Additionally, the [cupy](https://cupy.dev/) package is required, and a compatible GPU must be available on the machine to run Cupy efficiently. Make sure to check your GPU compatibility with Cupy and install the necessary GPU drivers if needed.

```bash
pip install networkx cupy
```


## Parameters

The `lle_cupy(graph, dim)` function takes two parameters. The first parameter is a NetworkX graph, and the second parameter is the user-defined embedding dimension. It is important to note that the graph must be connected for the LLE algorithm to be applied successfully.

## Usage

To utilize the LLE implementation, call the `lle_cupy` function with a connected NetworkX graph and the desired embedding dimension.

```python
from LLE_Cupy import lle_cupy

# Example usage
graph = ...  # Your connected NetworkX graph
embedding_dimension = ...  # Your desired embedding dimension
embedding_result = lle_cupy(graph, embedding_dimension)
```


