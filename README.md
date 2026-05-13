# 🐔 Broiler Feed Optimization using Lexicographic Fuzzy Goal Programming (LFGP)

## 📌 Project Overview

This repository contains computational models, datasets, and research
findings for optimizing broiler chicken feed formulation in the poultry
industry.

Traditional feed formulation methods often fail to simultaneously
balance: - Nutritional requirements - Physical feed quality - Economic
constraints - Worker safety

This project transforms feed manufacturing into a **dynamic, integrated
factory system** using a **Lexicographic Fuzzy Goal Programming (LFGP)**
framework.

The model integrates: - Nutrition science - Machine physics - Production
economics - Ergonomic safety

across three broiler growth stages: - Pre-Starter - Starter - Finisher

------------------------------------------------------------------------

## 🎯 Key Objectives (Lexicographic Hierarchy)

The model follows a strict preemptive priority structure:

1.  **Nutritional Adequacy & Safety**
    -   Ensures all formulations meet biological nutrient bounds
2.  **Pellet Durability Index (PDI)**
    -   Maximizes physical feed quality (target: 92%)
3.  **Production Cost Minimization**
    -   Optimizes total cost including:
        -   Raw materials
        -   Energy (steam)
        -   Labor
        -   Packaging
4.  **Ergonomic Safety**
    -   Uses the NIOSH Lifting Equation
    -   Minimizes Lifting Index (LI) during bagging operations

------------------------------------------------------------------------

## 🔬 Methodology & Architecture

### 📊 Analytic Hierarchy Process (AHP)

-   Validated priority structure using expert input
-   Nutritional Adequacy received **55.8% weight**, confirming dominance

### ⚙️ Statistical Engineering (Design of Experiments)

-   Conducted **2⁴ Full Factorial Design**
-   Factors analyzed:
    -   Temperature
    -   Moisture
    -   Particle size
    -   Throughput
-   Used Minitab for regression and Pareto analysis

### 🔁 Dynamic Shadow Pricing

-   Performed parametric cost sweeps
-   Enabled automatic ingredient substitution under price volatility

### 🧮 Optimization Engine (SLSQP)

-   Problem size: **54 variables**
-   Decomposed into **3 stage-wise models**
-   Solved using:
    -   `scipy.optimize.minimize`
    -   Sequential Least Squares Programming (SLSQP)

------------------------------------------------------------------------

## 📊 Key Results & Business Impact

### ✅ Optimization Performance

-   Pellet Quality Satisfaction: **94%**
-   Nutritional Adequacy: **82%**
-   Cost Optimization: **71%**

### ⚠️ Ergonomic Risk Detection

-   Baseline system (manual 50 kg bags):
    -   Lifting Index range: **2.76 -- 8.77**
    -   Indicates **severe safety violation**

### 🏗️ CapEx Intervention

-   Introduced:
    -   Gravity conveyors
    -   Scissor lifts

### 💰 ROI Analysis

-   Final Lifting Index: **0.9 (safe zone)**
-   Annual Savings: **₹5,50,000**
-   ROI: **122.2%**
-   Payback Period: **0.81 years**

------------------------------------------------------------------------

## 💻 Technologies & Tools

### 🐍 Python

-   Core modeling and optimization
-   Libraries:
    -   numpy
    -   scipy.optimize
    -   matplotlib

### 📊 Minitab

-   Experimental design (DoE)
-   Regression modeling
-   Pareto analysis

------------------------------------------------------------------------

## 🚀 Project Significance

This work demonstrates a shift from: \> Static cost minimization →
Intelligent, multi-objective industrial optimization

Key contributions: - Integration of ergonomics into supply chain
optimization - Real-time adaptability to market conditions - Bridging
manufacturing physics with operations research

------------------------------------------------------------------------

## 📂 Repository Structure (Suggested)

    ├── data/
    ├── models/
    ├── notebooks/
    ├── results/
    ├── src/
    └── README.md

------------------------------------------------------------------------

## 📜 License

This project is intended for academic and research purposes.
