# Optimization of an Interrail Itinerary

This repository contains an Operations Research project focused on the design and mathematical optimization of an Interrail travel itinerary in Southern Europe (Italy, Portugal, Spain, and France). 

The model aims to maximize the tourism value of the travel experience while respecting strict constraints regarding the economic budget, total time available, and logistical rules related to the Interrail Global Pass.

This project was developed for the *Optimization Methods in Business Analytics* course within the Master’s degree program in *Analytics and Data Science for Economics and Management* (A.Y. 2024/2025).

## Authors
* Luigina Bertolotti
* Isabella Cappiello
* Martina Pagan

## Project Structure
The repository is organized as follows:

* **`Opt_project.ipynb`**: Jupyter Notebook containing the implementation of the mathematical model in Python using the Pyomo library, alongside data management via Pandas.
* **`REPORT_OPTIMIZATION_Bertolotti_Cappiello_Pagan.pdf`**: The comprehensive academic report describing the scenario, data collection criteria (TripAdvisor, Budget Your Trip), detailed mathematical formulation, and sensitivity analysis.
* **`Optimization_ppt_Bertolotti_Cappiello_Pagan.pdf`**: Presentation slide deck used for the final project defense.
* **Data Files (`.xlxs`)**: Datasets containing the list of candidate cities with their respective tourism attraction scores, average daily costs, and the railway transit travel time matrix.

## Tech Stack & Tools
* **Programming Language:** Python
* **Mathematical Modeling:** Pyomo (solvers for Mixed-Integer Linear Programming - MILP)
* **Data Analysis & Graphics:** Pandas, NumPy, Matplotlib, NetworkX (for visualizing the optimal itinerary graphs)
* **Data Sourcing:** Integration of real-world metrics (Budget Your Trip for average daily destination costs)

## 📈 Model Features & Results
The mathematical model selects the optimal sequence of cities to visit and the respective length of stay in each. It includes:
* Constraints on the maximum number of total travel days and effective train travel days (7 days within 1 month pass).
* Customizable budget limits with specific sub-constraints for accommodation, food, and transport.
* **Sensitivity Analysis:** An in-depth study of how variations in the overall budget and travel time penalty parameters ($\alpha$ and $\lambda$) impact the structure of the final itinerary, demonstrating the robustness and flexibility of the proposed model.
