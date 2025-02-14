# Crab Age Prediction Challenge

## 🦀 Overview
The Crab Age Prediction Challenge goal is to predict the age of crabs using regression models based on biological features. The project focuses on data preprocessing, feature scaling, and regularization techniques (L1, L2, and Elastic Net) to improve generalization. The model is evaluated using Mean Absolute Error (MAE) to ensure accuracy and robustness.

## 📂 Dataset Description
The dataset contains various biological features of crabs, such as:
- **Size-related attributes** (length, width, height, etc.)
- **Weight-related features** (whole weight, shell weight, etc.)
- **Other biological attributes**

### 🔍 Data Splits
- **Training Set**: Labeled dataset with features and corresponding ages.
- **Test Set**: Dataset with features but without age labels (participants submit predicted ages for evaluation).

## 🎯 Objective
Participants need to build a **regression model** that minimizes **Mean Absolute Error (MAE)** on the test set:

\[ MAE = \frac{1}{n} \sum_{i=1}^{m} |y - \hat{y}| \]

## 🔄 Data Preprocessing
### 🏷️ Encoding
- **Categorical Encoding**: Label Encoding was used for the "Gender" column

### ⚖️ Standardization
- **Feature Scaling**: We apply **StandardScaler** to ensure all numerical features are on a similar scale, improving model convergence.

## 🏗️ Model and Regularization Techniques
To ensure robust predictions and prevent overfitting, we incorporate **regularization techniques**, such as:
- **L1 Regularization (Lasso Regression)**: Shrinks less important feature weights to zero.
- **L2 Regularization (Ridge Regression)**: Reduces overfitting by penalizing large coefficients.
- **Elastic Net**: A combination of L1 and L2 regularization.

## 📊 Visualizations and Plots
- **Feature Distribution Plots**: Histograms and KDE plots to visualize feature distributions.
- **Correlation Matrix (Heatmap)**: Identifies relationships between variables.
- **Pair Plots**: Examines feature interactions.
- **Residual Plots**: Checks the regression model’s error distribution.
- **MAE Trend Analysis**: Line plots showcasing model performance across iterations.
