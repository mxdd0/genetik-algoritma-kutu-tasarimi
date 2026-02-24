# Cargo Box Optimization using Genetic Algorithm (Scenario 6)

This project was developed as part of the **BLG-307 Artificial Intelligence Systems** course.
* **Student:** Bahadır Beldek
* **Student ID:** 2112721066

## Project Description
This project aims to find the optimal cargo box dimensions (width and height) for an e-commerce company using a **Genetic Algorithm**. The objective is to maximize the volume while minimizing the material cost.

* **Selected Scenario:** Scenario 6
* **Objective Function:** `y = x1*x2 - 0.1*x1^2 - 0.1*x2^2`

### Variables
* **x1 (Width):** [10, 40] cm
* **x2 (Height):** [5, 20] cm

### Constraints
* **Shelf Limit:** `x1 * x2 <= 600`
* **Minimum Width:** `x1 >= 15`

## Methods Used
The project is implemented in Python, utilizing the following Genetic Algorithm mechanisms:
* **Population Size:** 50 Individuals
* **Selection:** Tournament Selection
* **Crossover:** Single-Point / Uniform Crossover
* **Mutation:** Random value assignment (10% mutation rate)
* **Penalty Method:** Individuals failing to meet the constraints are severely penalized (score: -9999) to ensure their elimination from the gene pool.

## Installation and Execution
1. Download the `.ipynb` file from this repository.
2. Open the file using **Google Colab** or **Jupyter Notebook**.
3. Run all cells sequentially.

## Results
The algorithm successfully identifies the best `x1` and `x2` values that satisfy all constraints. The evolutionary progress of the population across generations is also visualized via an output graph.
