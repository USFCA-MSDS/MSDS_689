# Homework Assignment: Exploring K-Means Algorithm

## Objective
- Implement K-Means clustering using object-oriented programming in Python.
- Explore the algorithm's complexity in terms of time and space with respect to its variables.
- Apply K-Means for image compression by mapping pixel space into $R^3$ and reducing the number of colors.

## Task 1: Implementing K-Means Algorithm 
1. Write a Python class named `KMeans` that encapsulates the K-Means clustering algorithm.
2. Ensure your code follows PEP 8 style guidelines, including proper indentation, spacing, and line lengths.
3. Use meaningful variable names that convey the purpose of each variable.
4. Include docstrings for class, methods, and significant blocks of code.
5. Implement a thorough set of tests for your K-Means implementation using a testing library like `unittest` or `pytest`.
6. Consider edge cases and unexpected inputs in your testing strategy.

for the above task you can start with the signature :


```python
import numpy as np

class KMeans:
    def __init__(self, n_clusters=3, max_iterations=100, random_state=None):
        """
        Initialize KMeans clustering algorithm.

        Parameters:
        - n_clusters: Number of clusters (default is 3).
        - max_iterations: Maximum number of iterations (default is 100).
        - random_state: Seed for random number generation (default is None).
        """
        self.n_clusters = n_clusters
        self.max_iterations = max_iterations
        self.random_state = random_state
        self.centroids = None
        self.labels = None

    def fit(self, data):
        """
        Fit the KMeans algorithm to the input data.

        Parameters:
        - data: Numpy array of shape (m, n) representing m data points in an n-dimensional space.
        """
        # Implementation of KMeans algorithm

    def predict(self, data):
        """
        Assign data points to the nearest cluster based on current centroids.

        Parameters:
        - data: Numpy array of shape (m, n) representing m data points in an n-dimensional space.

        Returns:
        - labels: Array of cluster labels assigned to each data point.
        """
        # Implementation of data point assignment

    def get_centroids(self):
        """
        Get the current centroids after fitting the algorithm.

        Returns:
        - centroids: Numpy array representing the centroids of clusters.
        """
        return self.centroids
```

## Task 2: Complexity Exploration
1. Analyze the time complexity of your K-Means implementation. Consider the impact of the number of points (`m`), clusters (`K`), iterations (`I`), and attributes (`n`). These variables are explained in the [lecture](https://github.com/USFCA-MSDS/MSDS_689/blob/main/lectures/K_means_lecture.pdf).
2. Implement experiments to measure the running time for varying values of these parameters.
3. Create plots to visualize the growth in running time as each variable changes. Discuss the observed trends.

## Task 3: Image Compression using K-Means 
1. Choose a color image (e.g., PNG or JPEG) for image compression.
2. Convert the image to a NumPy array and reshape it to represent the pixel space.
3. Use the K-Means algorithm to cluster the pixels in R^3 space. Reduce the number of colors by replacing each pixel with its cluster centroid.
4. Display the original and compressed images side by side. Discuss the visual impact of compression.

## Additional Tasks for Exploration 
1. Compare the K-Means algorithm's performance with different initialization strategies (e.g., random initialization).
2. Experiment with different distance metrics for assigning data points to clusters (e.g., Euclidean distance, Manhattan distance).

## Deliverables
1. A well-documented Python notebook (.ipynb) with clear explanations and code comments.
2. Visualization of K-Means clustering results and complexity analysis plots.
3. Display of the original and compressed images with a discussion of the compression results.
4. A separate testing script or section within the notebook demonstrating test coverage and reliability.

## Submission Guidelines
1. Submit the Python notebook via the designated platform.
2. Ensure the notebook includes all necessary explanations, code, visualizations, and testing sections.
3. The code should pass linting tools for PEP 8 compliance, and testing results should be included.

## Grading Criteria
- Implementation of K-Means class: 30 points
- Complexity exploration and analysis: 30 points
- Image compression using K-Means: 30 points
- Code quality, adherence to PEP 8, meaningful docstrings, and testing: 10 points

