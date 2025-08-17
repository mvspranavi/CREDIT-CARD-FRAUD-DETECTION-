# Enhancing-Credit-Card-Fraud-Detection-Models-using-Machine-Learning-and-PCA

## Overview
Credit card fraud detection is a critical issue for financial institutions as fraudulent activities result in significant financial losses annually. Traditional fraud detection systems often struggle to keep pace with increasingly sophisticated fraud schemes. This project focuses on enhancing fraud detection systems by integrating advanced machine learning techniques, addressing class imbalance, and reducing the dimensionality of transaction data.

## Objectives
1. Address class imbalance using the Synthetic Minority Over-sampling Technique (SMOTE) to ensure models can effectively learn from both fraudulent and non-fraudulent transactions.
2. Reduce the dimensionality of the dataset using Principal Component Analysis (PCA) to enhance computational efficiency and improve model accuracy.
3. Build and evaluate machine learning models such as Logistic Regression, Random Forest, and Neural Networks to identify fraudulent transactions.

## Key Findings
- Both the Neural Network and Random Forest models achieved perfect performance with an AUC-ROC score of 1.00.
- Logistic Regression performed well with an AUC-ROC score of 0.9923, offering a simpler alternative with high accuracy in resource-constrained environments.

This project demonstrates the importance of handling class imbalance and dimensionality reduction for robust fraud detection systems.


## Dataset
The dataset used for this project is sourced from Kaggle's Credit Card Fraud Detection dataset (Link - https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud ). It contains anonymized transaction data from European cardholders and includes 284,807 transactions, of which 492 are fraudulent. The dataset is heavily imbalanced, which is addressed using SMOTE.

## Installation

Clone this repository:
```bash
git clone https://BalaElangovan/Enhancing-Credit-Card-Fraud-Detection-Models-using-Machine-Learning-and-PCA.git
cd Enhancing-Credit-Card-Fraud-Detection-Models-using-Machine-Learning-and-PCA
```

Install the necessary dependencies:

```bash
pip install -r requirements.txt
```

Run the Jupyter notebooks for an in-depth analysis and model evaluation:

```bash
Copy code
jupyter notebook notebooks/Main.ipynb
```

## Key Features
- **SMOTE:** Synthetic Minority Over-sampling Technique is used to tackle the class imbalance problem.
- **PCA:** Principal Component Analysis reduces the dimensionality of the dataset, improving computational efficiency and model performance.
- **Machine Learning Models:** Includes Logistic Regression, Random Forest, and Neural Networks, evaluated for their precision, recall, F1-score, and AUC-ROC.

## Visualization
### 1. Class Distribution Plot
This visualization shows the balanced dataset after applying SMOTE, which is critical for handling class imbalance in fraud detection.

### Class Distribution
![Class Distribution](https://github.com/BalaElangovan/Enhancing-Credit-Card-Fraud-Detection-Models-using-Machine-Learning-and-PCA/blob/main/charts/4.png)

The dataset was heavily imbalanced, with fraudulent transactions being a minority. The Synthetic Minority Over-sampling Technique (SMOTE) was used to balance the dataset, as shown above.

### 2. Transaction Amount Distribution Plot
This plot shows the distribution of transaction amounts, which is important for understanding the nature of the dataset.

### Transaction Amount Distribution
![Transaction Amount Distribution](https://github.com/BalaElangovan/Enhancing-Credit-Card-Fraud-Detection-Models-using-Machine-Learning-and-PCA/blob/main/charts/5.png)

The dataset contains a wide range of transaction amounts, and this feature plays a key role in identifying patterns that may indicate fraudulent activity.

### 3. Correlation Heatmap
This heatmap highlights the correlation between features, helping to visualize how different variables relate to one another.

### Correlation Heatmap
![Correlation Heatmap](https://github.com/BalaElangovan/Enhancing-Credit-Card-Fraud-Detection-Models-using-Machine-Learning-and-PCA/blob/main/charts/6.png)

Principal Component Analysis (PCA) was applied to reduce dimensionality, focusing on the most relevant features as shown in the correlation heatmap.

### 4. ROC Curve
ROC curves for different models (Logistic Regression, Random Forest, and Neural Network) demonstrate the model's ability to classify transactions correctly.

### ROC Curve
![ROC Curve](https://github.com/BalaElangovan/Enhancing-Credit-Card-Fraud-Detection-Models-using-Machine-Learning-and-PCA/blob/main/charts/10.png)

The models' ROC curves show the performance of Logistic Regression, Random Forest, and Neural Networks. Both Random Forest and Neural Networks achieved perfect classification (AUC-ROC = 1.00).

### 5. Confusion Matrices
Confusion matrices show the classification performance for each model, providing a clear view of how well each model identifies fraud vs. non-fraud transactions.

### Confusion Matrix
- **Logistic Regression**
![Confusion Matrix - Logistic Regression](https://github.com/BalaElangovan/Enhancing-Credit-Card-Fraud-Detection-Models-using-Machine-Learning-and-PCA/blob/main/charts/11.png)

- **Random Forest**
![Confusion Matrix - Random Forest](https://github.com/BalaElangovan/Enhancing-Credit-Card-Fraud-Detection-Models-using-Machine-Learning-and-PCA/blob/main/charts/12.png)

The confusion matrices above display the true positive, false positive, true negative, and false negative results for each model.
By incorporating these visualizations, you make it easier for readers to understand the impact of your preprocessing steps and the performance of your models.

## Results
- **Random Forest and Neural Networks:** Both models achieved an AUC-ROC score of 1.00, providing near-perfect accuracy in identifying fraudulent transactions.
- **Logistic Regression:** Achieved an AUC-ROC score of 0.9923, offering a balance of performance and computational efficiency.

## Usage
To run the project, execute the Jupyter notebooks in the /notebooks directory. Each notebook walks through data preprocessing, feature engineering, model building, and evaluation.

## Evaluation Metrics
The models were evaluated using precision, recall, F1-score, and AUC-ROC to assess their ability to detect fraudulent transactions in an imbalanced dataset. Confusion matrices were used to further assess model performance.
