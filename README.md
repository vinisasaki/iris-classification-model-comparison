# Iris Species Classification with Model Comparison

This project uses the classic Iris dataset to develop and evaluate multiple machine learning models, with the goal of finding the most robust and accurate classifier to identify the flower species.

## 📜 Description

The Iris dataset contains 150 samples of three species of Iris flowers (*Iris setosa*, *Iris versicolor*, and *Iris virginica*). For each sample, four features are measured: the length and width of the sepals and petals. This project implements a complete machine learning workflow to solve this multi-class classification problem.

The main focus is the comparison of seven different classification algorithms, using cross-validation to ensure a fair and reliable evaluation of each one's performance.

## ✨ Features and Workflow

The project follows a structured workflow:
1.  **Data Loading and Cleaning:** Obtaining the dataset from the UCI repository and removing duplicate values.
2.  **Exploratory Data Analysis (EDA):** Visualizing the data to understand the relationships between features and the separability of the classes, using scatter plots, boxplots, and a correlation matrix.
3.  **Preprocessing:** Application of `StandardScaler` to scale the features, ensuring that scale-sensitive models have optimized performance.
4.  **Model Training and Evaluation:** Seven different algorithms were trained and evaluated:
    * Logistic Regression
    * K-Nearest Neighbors (KNN)
    * Support Vector Machine (SVM)
    * Decision Tree
    * Random Forest
    * Gradient Boosting
    * Naive Bayes
5.  **Validation:** Using Scikit-learn `Pipelines` in conjunction with Cross-Validation (K-Fold with 5 folds) to prevent data leakage and obtain a reliable performance estimate.
6.  **Results Analysis:** Final comparison of the average accuracy of each model to determine the most effective one.

## 🚀 How to Run
  
The easiest way to run this project is by opening the notebook directly in Google Colab. Click the badge below to open it in your browser.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vinisasaki/iris-classification-model-comparison/blob/main/iris-classification-comparison-models.ipynb)

## 📊 Results and Conclusion

After evaluation using cross-validation, the performance results of the models were as follows:

| Model | Average Accuracy (CV) |
| :--- | :--- |
| **Support Vector Machine** | 96.7% |
| **Random Forest** | 96.7% |
| Gradient Boosting | 96.0% |
| K-Nearest Neighbors | 96.0% |
| Logistic Regression | 96.0% |
| Naive Bayes | 95.3% |
| Decision Tree | 95.3% |

![Model Comparison Chart](images/comparison_graph)

**Final Conclusion:**

The **Support Vector Machine (SVM)** and **Random Forest** models were identified as the best-performing models, both achieving an **average accuracy of 96.7%**. 
The analysis also highlighted the importance of cross-validation as an essential technique for obtaining a reliable performance evaluation, correcting the potentially
misleading view that a single `train-test-split` can offer.


>  
> [LinkedIn](https://www.linkedin.com/in/vinicius-sasaki) • [GitHub](https://github.com/vinisasaki)  
