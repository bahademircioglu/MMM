# MMM (Marketing Mix Modelling) - Data Analysis and Regression Modeling Project

A Python-based data analysis and modeling project designed to process and analyze data from a given Excel file. The project includes cleaning, feature engineering, and applying statistical and machine learning regression models to predict and analyze outcomes.

---

## Features

- **Data Cleaning and Preprocessing:**
  - Replaces missing or invalid `USD_RATE` values using forward fill methodology.
  - Handles other potential data inconsistencies for smooth processing.

- **Feature Engineering:**
  - Calculates new columns such as:
    - `Competitor_Total_USD`, `Competitor1_USD`, `Competitor2_USD`, `Offline_Investment_USD`
    - `Total_Impressions`: Aggregates impressions from various platforms.
  - Adds dummy variables for the `Date` column to represent months as features.

- **Exploratory Data Analysis:**
  - Uses descriptive statistics and correlation matrices.
  - (Optional) Visualizations such as pair plots and heatmaps.

- **Regression Modeling:**
  - Implements Ordinary Least Squares (OLS) regression to evaluate relationships between features and target (`Sales`).
  - Applies Ridge, Lasso, and ElasticNet regression with hyperparameter tuning to optimize models.

- **Tree-Based Modeling:**
  - Builds a Decision Tree Regressor to evaluate feature importance and predictions.

- **Performance Metrics:**
  - Computes metrics such as Mean Squared Error (MSE) and R-squared for model evaluation.

---

## Prerequisites

- Python 3.x
- Required libraries:
  ```bash
  pandas numpy scikit-learn statsmodels matplotlib seaborn
  ```
- Input data file: `MMM_Data_Task(3123).xlsx`

---

## Usage

1. **Set Up Environment:**
   - Install the required libraries:
     ```bash
     pip install pandas numpy scikit-learn statsmodels matplotlib seaborn
     ```

2. **Prepare Input Data:**
   - Ensure the input Excel file (`MMM_Data_Task(3123).xlsx`) is in the same directory as the script.

3. **Run the Script:**
   - Execute the Jupyter Notebook or Python script to perform data analysis and regression modeling.

4. **Examine Outputs:**
   - View data insights, regression summaries, and feature importance rankings.
   - Interpret predictions and evaluation metrics.

---

## Workflow

1. **Data Cleaning:**
   - Replace zero values in `USD_RATE`.
   - Drop or encode categorical features where necessary.

2. **Feature Engineering:**
   - Create relevant features to enhance model performance.
   - Use dummy encoding for categorical data.

3. **Modeling and Tuning:**
   - Train and evaluate multiple regression models.
   - Tune hyperparameters for Ridge, Lasso, and ElasticNet regressions.

4. **Evaluation:**
   - Compare models using R-squared and RMSE values.
   - Identify the most predictive features using tree-based feature importance.

---

## Results

- **OLS Regression:** Adjusted R-squared of ~65% indicates moderate predictive capability.
- **Regularized Models:** Ridge and Lasso regressions achieved improved predictions after tuning.
- **Feature Importance:** Offline Investment showed minimal correlation with Sales, as per OLS analysis.
- **Tree-Based Models:** Highlighted key features contributing to predictions with interpretable visualizations. Also, Decision tree regression achieved ~84% rating with the parameter max depth=5.

---

## Future Work

- **Visualization Enhancements:**
  - Integrate advanced plotting for clearer data representation.
- **Automation:**
  - Automate hyperparameter tuning and model selection for scalability.
- **Deployment:**
  - Package as a web app for end-user interaction.

---

## License

This project is licensed under the GPL License. See the LICENSE file for details.

---

## Contribution

Contributions are welcome! Fork this repository and submit pull requests to suggest improvements or new features.

---

## Contact

For queries or support, please reach out via the Issues section on the GitHub repository.

