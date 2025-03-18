# Liver Cirrhosis Prediction Using ML models

This project performs an end-to-end analysis to predict liver cirrhosis using machine learning techniques. The notebook covers everything from dataset analysis and preprocessing to model training, evaluation, and visualization.

## Overview

- **Dataset Analysis:**  
  Load and inspect the dataset to understand its structure, data types, missing values, and basic statistics.

- **Data Preprocessing:**  
  Handle missing values, convert categorical data to numerical formats, and scale features for optimal model performance.

- **Exploratory Data Analysis (EDA):**  
  Generate visualizations such as regression plots, bar plots, and heatmaps to examine feature relationships and model performance.

- **Model Implementation:**  
  Train and evaluate three models: Logistic Regression, K-Nearest Neighbors (KNN), and Random Forest.

- **Results Visualization:**  
  Compare model accuracies with a bar plot and visualize confusion matrices using heatmaps.

## Project Structure

```
.
├── README.md                        # Project documentation
├── liver_cirrhosis_data.csv         # Dataset file (example)
└── liver_cirrhosis_pred.ipynb       # Jupyter Notebook containing all code
```

## Requirements

- Python 3.x
- Jupyter Notebook or JupyterLab
- Libraries:
  - pandas
  - numpy
  - matplotlib
  - seaborn
  - scikit-learn

You can install the required packages with:

```bash
pip install -r requirements.txt
```

## How to Run

1. **Clone the repository:**

   ```bash
   git clone https://github.com/morbidflames/liver_cirrhosis_pred.git
   ```

2. **Navigate to the project directory:**

   ```bash
   cd liver_cirrhosis_pred
   ```

3. **Ensure the dataset file (`liver_cirrhosis_data.csv`) is in the directory.**

4. **Open the Jupyter Notebook:**

   ```bash
   jupyter notebook liver_cirrhosis_pred.ipynb
   ```

5. **Run the cells in the notebook to execute the analysis and model evaluation.**

## Data Preprocessing

- **Missing Value Handling:**  
  Missing data is addressed using a forward-fill strategy, ensuring continuity and reducing the risk of data loss.

- **Categorical Data Conversion:**  
  Categorical features are transformed into numerical values via one-hot encoding, making them compatible with machine learning models.

- **Feature Scaling:**  
  Numeric features are standardized using StandardScaler, ensuring that all variables contribute equally during model training.

## Exploratory Data Analysis (EDA)

- **Dataset Analysis:**  
  Provides insights into the dataset's columns, shape, initial rows, and basic statistics.

- **Regression Plots:**  
  Visualizes the relationship between each numeric feature and the target variable. The plots are arranged in rows of two to facilitate side-by-side comparisons.

- **Heatmaps:**  
  Displays correlation heatmaps for feature analysis and confusion matrix heatmaps for evaluating model performance.

## Model Implementation and Evaluation

- **Data Splitting:**  
  The dataset is split into training and testing sets with stratification for balanced class representation.

- **Model Training:**  
  Three models are implemented:
  - **Logistic Regression:** Evaluated using accuracy, confusion matrix, and classification report.
  - **KNN Model:** Uses 10 neighbors for classification.
  - **Random Forest Model:** Configured with 100 estimators, a maximum depth of 12, and a random state of 0.

- **Result Visualization:**  
  Model accuracies are compared using a bar plot, and confusion matrix heatmaps provide a detailed look at prediction errors and overall performance.

## Conclusion
The project successfully demonstrates the prediction of liver cirrhosis stages using machine-learning models. The Random Forest model is the best-performing model in this experiment.

