# Predicting Structural Fatigue Using Vibration Signals

This capstone practicum, sponsored by **Sandia National Laboratories**, explores how machine learning and deep learning can detect **early signs of structural fatigue** in critical systems like aircraft engines. Using the NASA C-MAPSS dataset, the project aimed to predict the **Remaining Useful Life (RUL)** of components and provide insights for predictive maintenance.

## Project Overview

* **Problem:** Structural fatigue in engines and turbines leads to costly downtime and potential safety risks.
* **Goal:** Develop predictive models that estimate RUL and flag components nearing failure.
* **Approach:**

  * Preprocessed vibration signal data from NASA’s C-MAPSS FD001 dataset.
  * Conducted **exploratory data analysis** (correlation, PCA, degradation trajectories).
  * Built baseline **Random Forest regressors** for RUL prediction.
  * Developed advanced **sequence models**: GRUs, LSTMs, and an attention-based LSTM.
  * Explored a **binary classification model** to flag engines at critical risk.

## Key Results

* **Best Model:** An **Attention-LSTM** achieved the lowest error (RMSE ≈ 47.5) and improved interpretability by identifying critical time steps.
* **Random Forests:** Provided a baseline with moderate accuracy but failed to capture temporal dynamics.
* **Classification Model:** Achieved near-perfect validation accuracy but struggled on test data due to imbalance.
* **Impact:** Demonstrated that **temporal models outperform static ones** and that attention mechanisms enhance both accuracy and explainability.

## Skills Demonstrated

* **Time-Series Modeling:** GRUs, LSTMs, attention mechanisms for sequential sensor data.
* **Machine Learning:** Random Forests, PCA, hyperparameter optimization (Optuna).
* **Data Preprocessing:** Scaling, redundancy reduction, sequence generation.
* **Evaluation:** RMSE, MAE, R², confusion matrices, class imbalance handling with SMOTE.
* **Communication:** Produced a final report and sponsor presentation with actionable insights.

## Tools & Technologies

* Python (NumPy, Pandas, scikit-learn, TensorFlow/Keras, Optuna)
* Jupyter Notebooks (`EDA.ipynb`, `Modeling.ipynb`)
* Tableau (for initial exploratory visualizations)

## Repository Contents

* **`Egret_Diane_Final_Report.pdf`** – Full final report (methods, results, recommendations).
* **`EDA.ipynb`** – Exploratory data analysis and preprocessing.
* **`Modeling.ipynb`** – Machine learning and deep learning models.
* **`data/train_FD001.txt`** – Training dataset.
* **`data/test_FD001.txt`** – Test dataset.
* **`data/RUL_FD001.txt`** – Ground-truth RUL values for test set.

## Business Impact

* Supports **predictive maintenance** in aerospace and energy industries.
* Provides insights that can **reduce operational costs, prevent downtime, and improve safety**.
* Demonstrates how data science can connect engineering to decision-making.

## Credits

Capstone Practicum (MGT 6748) – **Georgia Tech**, Summer 2025

* Project by **Diane Egret**
* Sponsor: **Sandia National Laboratories**
* Advisor: Steven Smith
