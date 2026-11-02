# Decision Tree Regression – California Housing Dataset

## 📌 Project Overview

This project implements a **Decision Tree Regression** model using the California Housing Dataset to predict median house values based on different housing-related features.

The project demonstrates an end-to-end Machine Learning workflow, including data exploration, preprocessing, model building, prediction, evaluation, visualization, and hyperparameter experimentation.

It also explores how different Decision Tree parameters influence model performance and how overfitting can affect predictions on unseen data.

## 🎯 Project Objective

To build a Decision Tree Regressor that predicts median house values using housing-related features and evaluate its performance using different evaluation metrics and model configurations.

## 📊 Dataset Information

**Dataset:** California Housing Dataset

- Total Records: 20,640
- Total Columns: 9
- Input Features: 8
- Target Variable: `target`

The target variable represents the median house value.

## 🛠️ Technologies and Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## ⚙️ Project Workflow

### 1. Data Exploration
- Load the California Housing dataset.
- Examine dataset shape and column names.
- Display the first five records.
- Identify feature and target columns.
- Check missing values and data types.

### 2. Data Preprocessing
- Handle missing values using median imputation when required.
- Separate independent and dependent variables.
- Split the dataset into 80% training data and 20% testing data.
- Use `random_state=42` for reproducibility.

### 3. Model Building
- Implement the Decision Tree Regressor.
- Use `squared_error` as the initial splitting criterion.
- Train the model using training data.
- Generate predictions on testing data.

### 4. Model Evaluation

Evaluate model performance using:

| Metric | Purpose |
|---|---|
| R² Score | Measures the variation explained by the model |
| MAE | Measures average absolute prediction error |
| RMSE | Measures prediction error while penalizing larger errors |

### 5. Overfitting Analysis
- Compare training and testing R² scores.
- Identify overfitting by analyzing the performance difference.
- Understand how model complexity affects generalization.

### 6. Maximum Depth Experimentation

Compare Decision Tree models using different `max_depth` values:

- `max_depth=3`
- `max_depth=7`
- `max_depth=None`

Evaluate training and testing performance to understand the effect of tree depth.

### 7. Decision Tree Visualization
- Identify the best-performing maximum depth among the tested models.
- Visualize the selected Decision Tree.
- Understand how the model makes predictions through decision rules.

### 8. Splitting Criteria Comparison

Compare two splitting criteria:

- `squared_error`
- `absolute_error`

Analyze their impact on training and testing performance.

### 9. Hyperparameter Experimentation

Experiment with different `min_samples_leaf` values:

- 1
- 5
- 10
- 20

Compare training and testing R² scores to understand how leaf size affects model complexity and generalization.

## 📈 Key Observations

- Decision Trees can capture non-linear relationships in data.
- Feature scaling is not required for Decision Tree models.
- Deep Decision Trees can overfit training data.
- Comparing training and testing performance helps identify overfitting.
- Maximum depth controls the complexity of the tree.
- Different splitting criteria can influence model performance.
- Adjusting `min_samples_leaf` can help control tree complexity.

## 💻 How to Run the Project

1. Clone this repository:

   ```bash
   git clone <your-repository-url>
   ```

2. Navigate to the project folder:

   ```bash
   cd decision-tree-regression-california-housing
   ```

3. Install the required libraries:

   ```bash
   pip install pandas numpy matplotlib scikit-learn openpyxl jupyter
   ```

4. Ensure the dataset file `fetch_california_housing.xlsx` is available in the project directory.

5. Open Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

6. Open and execute the Decision Tree Regression notebook.

## 🎓 Learning Outcomes

Through this project, I gained practical understanding of:

- Regression using Decision Trees.
- Data exploration and preprocessing.
- Model training and prediction.
- Regression evaluation metrics.
- Overfitting and generalization.
- Decision Tree visualization.
- Hyperparameter experimentation.
- Comparing model configurations.

## 👩‍💻 Author

**Marishetty Ramyakrishna**

Machine Learning | Python | Data Science

---

⭐ If you find this project useful, feel free to explore the repository!
