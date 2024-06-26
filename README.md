# Predicting movie success

## Overview
This Python program performs classification to predict the success of movies based on various features extracted from a movie dataset. The success of movies is categorized into three classes: "FLOP," "AVG," or "HIT," based on IMDb scores. The classification model is built using the Random Forest algorithm and incorporates feature engineering techniques like feature selection and scaling.

## Features
- **Data Reading**: The program reads a movie dataset from a CSV file using Pandas.
- **Target Variable Categorization**: IMDb scores are categorized into bins to represent movie success levels and visualized using a bar plot.
- **Handling Missing Values**: Missing values in the dataset are identified and dropped.
- **Descriptive Statistics**: Descriptive statistics for categorical columns are provided.
- **Label Encoding**: Categorical columns are encoded using label encoding for numerical representation.
- **Correlation Analysis**: The correlation matrix between variables is calculated and visualized using a heatmap.
- **Classification Model Building**:
  - **Data Splitting**: The dataset is split into independent variables (X) and the target variable (y).
  - **Scaling**: Independent variables are scaled using StandardScaler.
  - **Feature Selection**
  - Elimination with Cross-Validation (RFECV) is performed using a Random Forest classifier to select the optimal number of features.
  - **Training the Model**: A Random Forest classifier is trained on the selected features.
  - **Predicting the Target Variable**: The trained model is used to predict the target variable on the test data.
  - **Evaluation**: Confusion matrix and classification report are generated to evaluate the model's performance.

## How to Use
1. Ensure you have Python installed on your system.
2. Clone or download the repository to your local machine.
3. Install the required dependencies by running:
4. Run the Python script `movie_success_prediction.py`.
5. The program will read the dataset, perform data preprocessing, build the classification model, and evaluate its performance.
6. Review the generated confusion matrix and classification report to assess the model's accuracy.

## Dataset
IMDB 5000 Movie Dataset
link:- https://www.kaggle.com/datasets/carolzhangdc/imdb-5000-movie-dataset

## Dependencies
- numpy
- pandas
- matplotlib
- seaborn
- scikit-learn
