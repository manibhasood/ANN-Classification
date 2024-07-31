# ANN Binary Classification on Gaussian Clusters

This project implements an Artificial Neural Network (ANN) to perform binary classification on two Gaussian clusters. Our model achieves an impressive overall accuracy of 94.5%.

## Dataset Overview

The dataset is synthetically generated with the following characteristics:

- Two clusters (A and B) with Gaussian distribution
- 100 points per cluster
- 2D feature space
- Controllable cluster separation and noise

## Data Generation Parameters

- `nPerClust`: 100 (number of points per cluster)
- `blur`: 1 (standard deviation of Gaussian noise)
- Cluster A center: [1, 1]
- Cluster B center: [5, 1]

## Project Goals

1. Generate synthetic data for binary classification
2. Implement an ANN using PyTorch
3. Train the model to distinguish between two clusters
4. Achieve high classification accuracy (currently 94.5%)

## Tools and Libraries

- Python
- PyTorch for building and training the ANN
- NumPy for data generation
- Matplotlib for data visualization (if applicable)

## Model Performance

Our ANN model achieves an overall accuracy of 94.5% in classifying points between the two Gaussian clusters.

## Getting Started

1. Clone this repository
2. Install required dependencies
3. Run `ANN_classification.ipynb` to generate data, train the model, and see results

## Key Files

- `ANN_classification.ipynb`: Main script for data generation, model definition, training, and evaluation

## Model Architecture
Our ANN model is implemented using PyTorch's `nn.Sequential` and consists of the following layers:

    Linear(2, 1)  # input layer
    ReLU()        # activation unit
    Linear(1, 1)  # output unit
    Sigmoid()      # final activation unit

## Future Improvements

- Experiment with different network architectures
- Implement cross-validation for more robust performance estimation
- Extend the model to handle multiple clusters or higher-dimensional data
- Create a visualization of the decision boundary

## License

This project is licensed under the [MIT License]
