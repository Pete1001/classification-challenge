# classification-challenge
Module 13-SPAM detection challenge

# Spam Email Detection with Logistic Regression and Random Forest

## Overview

This project develops a machine learning-based email spam detection system using two supervised classification models: Logistic Regression and Random Forest. The goal is to compare these models' performance and determine which is more effective at detecting spam emails.

The dataset used for this project contains email data with labels indicating whether the email is spam (`1`) or not spam (`0`). The features include various attributes of the emails, and the dataset is sourced from the [Machine Learning Library](https://static.bc-edx.com/ai/ail-v-1-0/m13/challenge/spam-data.csv).

## Features

1. **Logistic Regression Model**: A linear classification model designed for binary outcomes, known for its simplicity and interpretability.
2. **Random Forest Model**: An ensemble-based classification model capable of handling non-linear relationships and feature interactions.
3. **Model Comparison**: Detailed evaluation of both models based on accuracy metrics.

## Results

- **Random Forest**: Achieved an accuracy of **95.8%**.
- **Logistic Regression**: Achieved an accuracy of **92.3%**.
- **Conclusion**: Random Forest outperformed Logistic Regression in this spam classification task, as predicted.

## Files

1. Initial code template to get started with the project.
2. `spam_detector.ipynb`: Completed Jupyter Notebook with the full implementation of the spam detection system.

## How to Run the Project

1. Clone the repository:
    ```bash
    git clone https://github.com/Pete1001/classification-challenge.git
    ```

2. Navigate to the project directory:
    ```bash
    cd classification-challenge
    ```

3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```
    Requirements:
        -pandas
        -scikit-learn

4. Open the Jupyter Notebook to explore the project:
    ```bash
    jupyter notebook spam_detector.ipynb
    ```

## Methodology

### 1. Data Preparation
- The dataset is loaded using Pandas and split into features (`X`) and labels (`y`).
- The `train_test_split` function is used to divide the data into training and testing sets.

### 2. Feature Scaling
- StandardScaler is applied to scale the features for better performance of machine learning models.

### 3. Model Implementation
#### Logistic Regression
- A linear classifier trained on scaled data using the `LogisticRegression` class from scikit-learn.
- Predictions are made using the test data.

#### Random Forest
- An ensemble classifier trained on scaled data using the `RandomForestClassifier` class from scikit-learn.
- Predictions are made using the test data.

### 4. Model Evaluation
- Both models are evaluated using the `accuracy_score` function from scikit-learn.
- The model with the higher accuracy score is deemed the better performer.

## Conclusion

The Random Forest model, with its ability to handle complex and non-linear data relationships, performed better than Logistic Regression in this spam classification task. However, Logistic Regression remains a viable choice for scenarios requiring simplicity and interpretability.

## License

This project is licensed by Pete Link.

## Author

- **[Pete Link]**

For any questions, feel free to contact [https://www.linkedin.com/in/petelink/].
