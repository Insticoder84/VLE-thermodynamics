# Data-Driven Thermodynamic Regression & Parameter Estimation Engine

## 📌 Project Overview
A computational thermodynamic tool developed in MATLAB that performs non-linear parameter estimation to model non-ideal binary Vapor-Liquid Equilibrium (VLE). Moving away from idealized textbook assumptions (Raoult's Law), this engine inputs raw, unaligned experimental lab data and applies numerical optimization to regress molecular interaction parameters and accurately locate azeotropic points.

## ⚙️ Core Engineering Principles Applied
* **Advanced Thermodynamics:** Utilizes Modified Raoult's Law coupled with the non-linear Van Laar Activity Coefficient model to capture severe deviations from ideality.
* **Mathematical Optimization:** Implements an optimization routine utilizing a Least-Squares Error objective function to minimize the Residual Sum of Squares (RSS) between empirical data and model predictions.
* **Numerical Regression:** Utilizes the multi-variable Nelder-Mead simplex algorithm (`fminsearch`) to iteratively compute optimal binary interaction parameters.

## 🚀 Key Features
* **Parameter Estimation:** Converts an explicit forward calculation into an inverse data-driven fitting problem, mimicking commercial process simulation engines like Aspen Plus.
* **Azeotrope Localization:** Automatically scans the generated phase equilibrium envelope to locate the precise coordinate where liquid and vapor compositions converge ($x_1 = y_1$).
* **Comparative Visualization:** Generates a high-resolution $P-x-y$ phase diagram mapping raw lab data points directly against the optimized bubble and dew point envelopes.

## 📊 Optimization & Regression Envelopes
The engine successfully regresses the data, matching literature physical benchmarks with extreme precision.

![Thermodynamic Model Fit](VLE_Regression_Plot.png)

## 🛠️ Technology Stack
* **Language:** MATLAB
* **Focus Area:** Process Modeling, Chemical Engineering Thermodynamics, Numerical Optimization, Parameter Regression.
