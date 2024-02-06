# Hierarchical Clustering with Euclidean Minimal Spanning Tree

## Introduction
Hierarchical Clustering (HC) is a powerful technique used in data science for grouping similar data points together. One common approach to HC involves using the Euclidean Minimal Spanning Tree algorithm to construct a hierarchical structure based on the distances between data points. In this repository, we provide helper [code](https://github.com/USFCA-MSDS/MSDS_689/blob/main/notebooks/hierarchical_clustering_using_MST.ipynb) for implementing HC using the Euclidean Minimal Spanning Tree algorithm.

### Euclidean Minimal Spanning Tree
The Euclidean Minimal Spanning Tree is a tree-like structure that connects all the data points in a dataset while minimizing the total edge weight. It is computed using the Union Find data structure and the Kruskal's algorithm for finding minimal spanning trees. The Union Find data structure efficiently maintains disjoint sets of objects and is particularly useful in the context of HC for merging clusters of data points.

### Computation Using Provided Method
The computation of the Euclidean Minimal Spanning Tree is facilitated by the provided helper [code](https://github.com/USFCA-MSDS/MSDS_689/blob/main/notebooks/hierarchical_clustering_using_MST.ipynb). The code includes functions for calculating the distances between data points, constructing the minimal spanning tree using Kruskal's algorithm, and performing hierarchical clustering based on the tree structure.

## Deliverable
Students are expected to use the provided helper [code](https://github.com/USFCA-MSDS/MSDS_689/blob/main/notebooks/hierarchical_clustering_using_MST.ipynb) to write an object-oriented implementation of Hierarchical Clustering. The deliverable should be a single notebook file (.ipynb) containing the implementation, documentation, and unit tests.

## Grading Criteria
To ensure the quality of the submissions, the homework assignment will be graded based on the following criteria:

1. **Functionality (50%)**: Correct implementation of Hierarchical Clustering using the Euclidean Minimal Spanning Tree algorithm.
2. **Documentation and Comments (20%)**: Clear documentation with comments and docstrings explaining the code's purpose and usage.
3. **Unit Tests (20%)**: Comprehensive unit tests to validate the functionality of the implementation.
4. **Code Structure and Readability (10%)**: Well-organized code structure and readability following PEP 8 guidelines.
