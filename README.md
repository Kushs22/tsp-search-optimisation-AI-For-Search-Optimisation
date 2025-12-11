 Travelling Salesman Problem – AI Search & Optimisation

Hill Climbing vs Genetic Algorithm
Author: Kush Sharma
Module: AI for Search & Optimisation (MSc Artificial Intelligence, UWE Bristol)

 Project Overview

This project implements and compares two optimisation techniques — Steepest Ascent Hill Climbing and a Genetic Algorithm (GA) — to solve the Travelling Salesman Problem (TSP) using a dataset of 50 cities.

The aim is to analyse:

Solution quality

Runtime efficiency

Algorithm behaviour as problem size increases

Trade-offs between local and global search strategies

All experiments were performed in Python (Jupyter Notebook) following PEP8 guidelines.

 Objectives

Load and validate TSP coordinate data

Compute a Euclidean distance matrix

Implement Hill Climbing (local search)

Implement Genetic Algorithm (global search)

Evaluate performance across different city counts (10–50)

Generate plots for runtime and solution quality

Visualise the best 50-city route

📂 Repository Structure
📁 TSP-Optimisation-Project
│
├── Travel Salesman Problem.ipynb        # Main Jupyter Notebook
├── cities.csv                            # Dataset of 50 city coordinates
├── tsp_results.csv                       # Results from all experiment runs
├── best_50_city_route.csv                # Final best route from GA
├── README.md                             # Project documentation (this file)
└── plots/                                # (Optional) Save graphs here

 Setup Instructions
1. Clone the Repository
git clone https://github.com/yourusername/TSP-Optimisation-Project.git
cd TSP-Optimisation-Project

2. Install Dependencies
pip install numpy pandas matplotlib

3. Open the Notebook
jupyter notebook "Travel Salesman Problem.ipynb"

-> How to Run the Project

Inside the notebook:

Run Cell 1 → Imports libraries, sets reproducibility seed.

Run Cell 2 → Loads CSV dataset and validates structure.

Generate distance matrix (Euclidean).

Run Hill Climbing (single + multiple runs).

Run Genetic Algorithm (selection, crossover, mutation, elitism).

Run experiments for 10, 20, 30, 40, 50 cities.

Generate plots for runtime vs problem size & tour length vs problem size.

Visualise best 50-city route.

📊 Results Summary
1️⃣ Hill Climbing

Fastest algorithm

Performs well for small problem sizes

Struggles with larger city counts due to local optima

2️⃣ Genetic Algorithm

More computationally expensive

Achieves shorter tour lengths for larger instances

Better global search through crossover & mutation

Trade-off:

Hill Climbing = Speed
Genetic Algorithm = Solution Quality

📈 Visual Outputs

The notebook generates:

Average Tour Length vs Problem Size

Average Runtime vs Problem Size

Best 50-City Route Visualisation

These visuals support the comparison and clearly show algorithm behaviour trends.

🗂️ Files Explained
File	Description
Travel Salesman Problem.ipynb	Full implementation & experiments
cities.csv	City coordinate dataset
tsp_results.csv	Logged performance metrics from experiments
best_50_city_route.csv	GA-generated best TSP tour for 50 cities
README.md	Project documentation
📚 Technologies Used

Python

NumPy

Pandas

Matplotlib

Jupyter Notebook

🙌 Acknowledgements

Supervision & academic guidance: UWE Bristol – AI for Search & Optimisation

Assistance for explanation clarity & structuring:
OpenAI ChatGPT (1–7 December 2025)

📝 License

This project is for educational and academic use only.


