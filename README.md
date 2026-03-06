# Queue-Aware Matheuristic EV Charging Scheduling with Supervised Service Time Calibration

## Overview

This project proposes a **queue-aware scheduling framework for electric vehicle (EV) charging stations** using machine learning and hybrid optimization techniques.

The system predicts EV charging service times using **Random Forest regression** and integrates the predictions into a **queueing-theory-based scheduling framework** to optimize charger allocation and reduce waiting times.

The optimization pipeline combines **Simulated Annealing, Genetic Algorithms, and Mixed Integer Programming** to improve system efficiency under uncertain demand conditions.

---

## Problem Statement

As electric vehicle adoption increases, charging stations often experience:

* Long waiting times
* Charger congestion
* Inefficient resource utilization

Traditional scheduling methods like **First-Come-First-Serve (FCFS)** fail to adapt to dynamic service times and stochastic arrivals.

This project introduces a **data-driven queue-aware scheduling framework** to improve EV charging station performance.

---

## Methodology

### 1. Data Preparation

* Dataset containing EV charging sessions
* Feature engineering and normalization
* Outlier removal using IQR

### 2. Service Time Prediction

Machine learning models used:

* Random Forest Regressor
* Gradient Boosting Regressor

Target variable:

* Charging service time

Evaluation metrics:

* Mean Squared Error (MSE)
* R² Score

---

### 3. Queue Modeling

Queue dynamics modeled using:

* **M/G/1 queue**
* **M/G/c multi-server queue**

Key metrics analyzed:

* Mean waiting time
* Queue length
* Charger utilization

---

### 4. Optimization Framework

Hybrid matheuristic optimization including:

* Simulated Annealing (SA)
* Genetic Algorithms (GA)
* Mixed Integer Programming (MIP)

Objective:

Minimize

Mean Waiting Time + Tail Delay (95th percentile)

---

## Results

Key performance improvements compared to FCFS scheduling:

* **27% reduction in mean waiting time**
* **43% reduction in tail delay**
* **15% increase in charger utilization**
* **70% reduction in optimization runtime**

---

## Repository Structure

```
ev-charging-matheuristic-optimization

data/
   ev_charging_dataset.csv

docs/
   EV_Charging_Project_Report.pdf

notebooks/
   ev_charging_optimization.ipynb

README.md
```

---

## Technologies Used

Python
Pandas
NumPy
Scikit-learn
Matplotlib
Queueing Theory
Simulated Annealing
Genetic Algorithms
Mixed Integer Programming

---

## Author

**Akhil Sebastian**

M.Tech Data Science
Amrita Vishwa Vidyapeetham

GitHub: https://github.com/akhilsebastian2000
LinkedIn: https://www.linkedin.com/in/akhilsebastian2000
