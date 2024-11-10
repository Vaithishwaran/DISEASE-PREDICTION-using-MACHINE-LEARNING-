# Diabetes prediction using machine learning

Import Libraries: Import essential libraries like pandas for data manipulation, seaborn and matplotlib for visualization, and sklearn for machine learning.

Load the Dataset: Read the CSV file using pd.read_csv() and store it in a DataFrame, df.

Data Cleanup: Drop the 'Group' column if it exists in the DataFrame to simplify the data.

Exploratory Data Analysis (EDA):

Use df.describe() and df.info() to inspect data summary and types.
Plot histograms for each feature to understand distributions.
Check class distribution to see how balanced the dataset is.
Outlier Removal:

Define a function to remove outliers using the IQR method.
Apply the function to specific columns (like 'Triceps', 'Pedigree', etc.) to clean the data.
Correlation Analysis:

Compute the correlation matrix using df.corr() and visualize it with a heatmap to see relationships between features.
Define Features and Target:

Separate the features (X) and the target variable (y) for classification.
Use columns like 'Glucose_concentration', 'BMI', etc., as features and 'Class' as the target.
Split the Dataset:

Split data into training and testing sets using train_test_split() with a 67-33 split.
Train Classifiers:

Train a DecisionTreeClassifier and a RandomForestClassifier on the training set.
Generate predictions on the test set for each classifier.
Evaluate Performance:

Compute confusion matrices, classification reports, and accuracy scores for both classifiers to compare their performance.
