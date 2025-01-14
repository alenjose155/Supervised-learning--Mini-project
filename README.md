# Supervised-learning--Mini-project
# Breast Cancer Classification Using Supervised Learning
# Overview
This project aims to classify breast cancer as malignant or benign using supervised learning techniques on the breast cancer dataset from the sklearn library. The project implements five classification algorithms and evaluates their performance to determine the best-suited model for this dataset.

# Dataset Description
The breast cancer dataset contains 30 numerical features derived from a digitized image of a fine needle aspirate (FNA) of a breast mass. The dataset has 569 samples, with each labeled as malignant (1) or benign (0).

# Preprocessing Steps
# 1. Loading the Data
The dataset was loaded directly from the sklearn.datasets library into a structured DataFrame for better analysis and visualization.

# 2. Exploratory Data Analysis (EDA)
# Dataset Overview: 
Basic statistics and structure of the dataset were examined using .info() and .describe().
# Class Distribution: 
The dataset's class distribution was visualized using a count plot, showing a slight class imbalance (62.7% benign, 37.3% malignant).
# Correlation Analysis: 
A heatmap was generated to visualize feature correlations. Features with high correlations (absolute correlation > 0.9) were identified to consider for dimensionality reduction or removal.
# Feature Distributions: 
Histograms for each feature were plotted to understand the spread and identify any skewness or outliers.
# 3. Handling Missing Values
Observation: The dataset contains no missing values, so no imputation was necessary.
# 4. Feature Scaling
# StandardScaler:
Applied to normalize all features by standardizing them to have a mean of 0 and a standard deviation of 1.
Justification: Algorithms like SVM and k-NN are sensitive to feature magnitudes. Scaling ensures fair contribution of all features to the model, improving performance.
# 5. Train-Test Split
Split Ratio: Data was split into 80% training and 20% testing sets for model training and evaluation.
Algorithms Implemented
# 1. Logistic Regression
Description: A linear model that uses a logistic function to map predicted values to probabilities. It is suitable for binary classification problems like this one.
Suitability: Its simplicity and interpretability make it a good baseline model for this dataset.
# 2. Decision Tree Classifier
Description: A tree-based model that splits the data into subsets based on feature thresholds, creating decision rules.
Suitability: It handles non-linear relationships and provides clear decision rules, which are helpful for understanding classification patterns.
# 3. Random Forest Classifier
Description: An ensemble of decision trees that aggregates their outputs to improve performance and reduce overfitting.
Suitability: It is robust to noise and can handle large datasets effectively, making it ideal for this task.
# 4. Support Vector Machine (SVM)
Description: SVM finds the optimal hyperplane that separates classes by maximizing the margin between them.
Suitability: It works well with high-dimensional data, such as this dataset, where feature scaling has been applied.
# 5. k-Nearest Neighbors (k-NN)
Description: A distance-based algorithm that classifies a data point based on the majority class of its k nearest neighbors.
Suitability: Its simplicity makes it a quick and effective method, but it requires scaling to ensure fair distance computation across features.
# Results and Observations
Each algorithm was evaluated using metrics such as accuracy, precision, recall, and F1-score. The Logistic Regression and SVM demonstrated the best performance, showcasing its robustness in handling complex patterns. 
