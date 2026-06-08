# SM_Letter
# Congestion-Aware Switch Migration for SDN Controller Load Balancing

This repository contains the implementation used for the letter titled:

**Congestion-Aware Routing-Based Dynamic Switch Migration for Controller Load Balancing in SDN**

The code evaluates controller load balancing under switch migration in Software-Defined Networking (SDN). The implementation compares the proposed congestion-aware migration model with two baselines.

## Algorithms Included

### 1. MCF-ARC

MCF-ARC is the proposed optimization-based switch migration approach. It jointly considers controller load balancing and routing feasibility using a multi-commodity-flow formulation over physical network arcs.

### 2. B1

B1 is an optimization-based baseline that performs switch migration for controller load balancing while considering migration-related cost terms.

### 3. B2 / EASM

B2 refers to the EASM heuristic baseline. It performs efficiency-aware switch migration based on controller load reduction and migration cost, without explicit multi-commodity routing constraints.

## Main Features

- SDN controller load-balancing through switch migration
- Controller capacity and overload handling
- Migration cost computation
- Congestion-aware routing feasibility for MCF-ARC
- Comparison with optimization and heuristic baselines
- Result generation for different network topologies and traffic settings
- CSV-based output for plotting and analysis

## Repository Structure

```text
.
├── data/                  # Input topology files or generated network data
├── results/               # Output CSV files and experiment results
├── plots/                 # Generated figures
├── src/                   # Source code for algorithms and experiments
├── run_experiments.py     # Main script to run experiments
├── plot_results.py        # Script for generating figures
└── README.md

## Repository Structure

```text
.
├── data/                  # Input topology files or generated network data
├── results/               # Output CSV files and experiment results
├── plots/                 # Generated figures
├── src/                   # Source code for algorithms and experiments
├── run_experiments.py     # Main script to run experiments
├── plot_results.py        # Script for generating figures
└── README.md
```

## Requirements

The code was developed and tested using:

- Python 3.x
- Gurobi Optimizer
- NumPy
- Pandas
- NetworkX
- Matplotlib

## Installation

Install the required Python packages:

```bash
pip install numpy pandas networkx matplotlib
```

## Note

Gurobi must be installed separately and a valid academic or commercial license must be activated before running the code.
