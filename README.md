# Pascal Assessment - QEPITA 2024

## Table of Contents
- [Introduction](#introduction)
- [How to Run](#how-to-run)
- [How It Works](#how-it-works)
- [Requirements](#requirements)
- [Contributors](#contributors)

---

## Introduction
This project is a solution to a graph-based problem where we compute and visualize the Maximum Independent Set (MIS) using a Python-based approach. The solution leverages the **Pulser** library for efficient graph management and **Matplotlib** for visualization.

The goal is to color the graph nodes by repeatedly applying the MIS algorithm, ensuring no connected nodes share the same color.

---

## How to Run

To run the program, follow these steps:

1. **Create a Virtual Environment**  
   Use the following command to create a virtual environment:
   ```bash
   python3 -m venv venv_name
   ```

2. **Activate the Virtual Environment**  
   Activate it using:
   ```bash
    source venv_name/bin/activate
   ```

3. **Install Required Packages**  
    Install the necessary dependencies:
   ```bash
    pip install pulser
    pip install pulser-core
   ```

## How It Works
1. **Declare Data**
    Start by defining the data for the problem:
    - The coordinates of nodes.
    - The radius of interference for each node.

2. **Build the Graph**
Using Pulser, construct the graph based on the input data. For better vizualisation, the graph is also visualized using Matplotlib.

3. **Define the MIS Solver**
Implement the Maximum Independent Set (MIS) solver, which identifies the largest set of nodes that are not connected to each other. This is a key step in solving the problem.

4. **Color the Graph**
Apply the MIS solver iteratively to color the graph.
Each iteration assigns a unique color to nodes removed by the MIS solver.
This ensures all adjacent nodes have distinct colors.