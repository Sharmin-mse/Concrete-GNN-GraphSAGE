# Concrete-GNN-GraphSAGE

This repository contains the source code used for the GraphSAGE-based prediction of concrete compressive strength.

## Source Code

The **Source code** folder contains two subfolders:

- **Transductive** – contains the original GraphSAGE models where the graph is constructed using the complete dataset before assigning the training, validation, and testing subsets.
- **Inductive** – contains the strict inductive models where the data are split first, and preprocessing and graph construction are performed using the training data only.

Both folders contain:

- Node-level Model A
- Node-level Model B
- Node-level Model C
- Node-level Model D
- Node-level Model E
- Graph-level Model A

## Model

GraphSAGE was implemented using PyTorch Geometric. Concrete mixture records are represented as nodes, and KNN is used to connect mixtures with similar compositions.

The models use a 70% training, 15% validation, and 15% testing split with a random seed of 42.

## Requirements

The main software packages used in this study include:

- Python
- PyTorch
- PyTorch Geometric
- scikit-learn
- NumPy
- pandas
- SciPy

## Running the Code

Download the UCI Concrete Compressive Strength dataset and update the dataset path in the corresponding notebook if necessary.

The notebooks can then be run sequentially from the first cell to the last cell.

**Note:** Due to differences in hardware, operating system, software environment, and library versions, the final numerical results may vary slightly from those reported in the manuscript. However, the overall trends and model behavior should remain consistent.

## Manuscript

This repository accompanies the manuscript:

**“Transforming Numerical Concrete Data into Graphs: A Graph Neural Network Framework for Concrete Strength Prediction.”**

Additional publication information will be added after publication.
