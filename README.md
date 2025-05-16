# Lookalike Clustering for Customer Segmentation: A Comparative Study of Quantum Annealing and Classical Algorithms

## Overview
This repository contains the dataset instances used in the paper *"Lookalike Clustering for Customer Segmentation: a Comparative Study of Quantum Annealing and Classical Algorithms"*.

## Repository Structure
- `instances/` - Contains the dataset instances used for experiments. Each instance represents a different customer segmentation problem.
- `README.md` - This file, providing an overview of the repository.


## Data Format
Each instance is stored in a JSON format with the following structure:
```json
{
  "distance_matrix": [
    {"229": 0.0, "253": 1.009, "284": 0.975, "211": 0.979, "155": 7.986},
    {"229": 1.009, "253": 0.0, "284": 1.337, "211": 1.149, "155": 8.248},
    {"229": 0.975, "253": 1.337, "284": 0.0, "211": 0.960, "155": 8.076},
    {"229": 0.979, "253": 1.149, "284": 0.960, "211": 0.0, "155": 8.310},
    {"229": 7.986, "253": 8.248, "284": 8.076, "211": 8.310, "155": 0.0}
  ],
  "idx_i0": [284],
  "points_to_add": 3,
  "selected_coordinates": [
    {"Dimensione_1": -2.721, "Dimensione_2": -0.380, "Cluster": "First"},
    {"Dimensione_1": -2.990, "Dimensione_2": -0.164, "Cluster": "First"},
    {"Dimensione_1": -2.825, "Dimensione_2": -0.011, "Cluster": "First"},
    {"Dimensione_1": -3.011, "Dimensione_2": 0.255, "Cluster": "First"},
    {"Dimensione_1": 4.997, "Dimensione_2": -0.395, "Cluster": "Second"}
  ]
}
```
### Explanation of Fields:
- **distance_matrix**: Distance matrix, where each entry represents the distance between customers.
- **idx_i0**: List of initial cluster points.
- **points_to_add**: Number of points to be added in the clustering process.
- **selected_coordinates**: Coordinates of selected points, each assigned to a cluster.
  - Points labeled as **"First"** belong to the same cluster as the initial point in **idx_i0**.
  - Points labeled as **"Second"** belong to the other cluster.

## Usage
Researchers and practitioners can use these instances to test clustering algorithms and compare performance between classical and quantum approaches. Example usage:

1. Clone the repository:
   ```bash
   git clone [https://github.com/your-repo/lookalike-clustering.git](https://github.com/regor-unimore/Lookalike-Clustering-for-Customer-Segmentation.git)
   ```
2. Load an instance file into your clustering framework.
3. Apply classical or quantum clustering algorithms.
4. Analyze and compare results.
