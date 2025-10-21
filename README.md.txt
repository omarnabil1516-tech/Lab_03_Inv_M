# Lot Sizing for Time-Varying Demand

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/omarnabil1516-tech/Lab_03_Inv_M/blob/main/Lot_Sizing_Analysis.ipynb)
<br>
*Note: The link above assumes your notebook file is named `Lot_Sizing_Analysis.ipynb` and is in the `main` branch.*

## Project Overview

This repository contains a Jupyter Notebook that implements, analyzes, and compares seven classic inventory lot-sizing policies for a single item with time-varying demand over a 12-month horizon. The goal is to determine the most cost-effective replenishment strategy by balancing ordering costs and inventory holding costs.

The analysis is based on a standard operations research problem with the following base-case parameters:
- **Ordering Cost (A):** $20
- **Unit Value (v):** $2/unit
- **Annual Carrying Cost Rate (r):** 0.24
- **12-Month Demand Forecast:** `[50, 70, 100, 120, 110, 100, 100, 80, 120, 70, 60, 40]`

## Implemented Policies

The notebook provides a complete implementation and cost analysis for the following policies:
1.  Fixed EOQ (Rounded to Months of Supply)
2.  Fixed Time Supply
3.  Cost per Unit Heuristic (Part Period Balancing)
4.  Silver-Meal Heuristic
5.  All-at-Once
6.  Lot-for-Lot
7.  **Bonus:** Wagner-Whitin Algorithm (Optimal Dynamic Programming solution)

## Features

-   **Detailed Plans:** Generates a month-by-month inventory plan for each policy, detailing orders, demand, and inventory levels.
-   **Cost Comparison:** Produces a summary table and a bar chart comparing the total costs of all policies, sorted to easily identify the best performers.
-   **Visualizations:**
    -   Inventory trajectory plot for the Silver-Meal policy.
    -   Gantt chart visualizing the optimal inventory coverage from the Wagner-Whitin plan.
-   **Interactive Dashboard:** Includes sliders to perform sensitivity analysis on key cost parameters (`A` and `r`) and see how the results change in real-time.
-   **Discussion & Insights:** Provides data-driven answers to the managerial questions from the original problem prompt.

## How to Use

### 1. Google Colab (Recommended)
-   Click the **Open in Colab** badge at the top of this README.
-   The notebook will open directly in your browser, ready to be executed cell by cell. No installation is required.

### 2. Local Environment
1.  Clone the repository:
    ```bash
    git clone https://github.com/omarnabil1516-tech/Lab_03_Inv_M.git
    ```
2.  Navigate into the project directory:
    ```bash
    cd Lab_03_Inv_M
    ```
3.  Install the necessary Python libraries:
    ```bash
    pip install pandas numpy matplotlib ipywidgets
    ```
4.  Launch Jupyter Notebook or JupyterLab:
    ```bash
    jupyter notebook
    ```
5.  Open the `Lot_Sizing_Analysis.ipynb` file.