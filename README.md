# Mushroom Edibility Prediction

This project explores supervised learning algorithms to predict whether mushrooms are edible or poisonous based on various features. The dataset used for this project is a cleaned version of a mushroom dataset, which includes 9 features such as cap diameter, cap shape, gill attachment, gill color, stem height, stem width, stem color, and season.

## Dataset

The dataset contains the following columns:

- `cap-diameter`
- `cap-shape`
- `gill-attachment`
- `gill-color`
- `stem-height`
- `stem-width`
- `stem-color`
- `season`
- `class` (Target class: 0 = edible, 1 = poisonous)

There are 24,360 instances of class 0 (edible) and 29,675 instances of class 1 (poisonous).
The dataset is credited to [@prishasawhney](https://www.kaggle.com/prishasawhney) from Kaggle.

## Objective

The main objective of this project is to build and evaluate supervised learning models to predict the edibility of mushrooms based on their features.

## Environment and Tools

- Python
- Jupyter Notebook / Google Colab
- Libraries: scikit-learn, numpy, matplotlib, pandas, seaborn, mglearn

## Installation

Ensure you have the following libraries installed: scikit-learn, numpy, matplotlib, pandas, seaborn, mglearn.

## Implementation

### Data Preprocessing

The data preprocessing steps include:

1. Handling missing values (assumed to be handled via Modal imputation).
2. One-hot encoding of categorical variables.
3. Standardizing numerical features.

### Models Used

- k-Nearest Neighbors (k-NN)
- Logistic Regression

### Evaluation Metrics

The models were evaluated using the following metrics:

- Precision
- Recall
- F1-Score
- Accuracy

## Results

### k-Nearest Neighbors (k-NN)

- **Precision:** 0.99 for both classes
- **Recall:** 0.99 for both classes
- **F1-Score:** 0.99 for both classes
- **Accuracy:** 98.93%

### Logistic Regression

- **Precision:** 0.72 for class 0, 0.77 for class 1
- **Recall:** 0.72 for class 0, 0.77 for class 1
- **F1-Score:** 0.72 for class 0, 0.77 for class 1
- **Accuracy:** 74.59%

### Model Comparison and Insights

- The k-NN model significantly outperformed the Logistic Regression model in all metrics.
- k-NN captured complex relationships in the data better than Logistic Regression.
- Logistic Regression might have suffered from underfitting due to its assumption of linear relationships.
- k-NN is computationally more expensive than Logistic Regression, which could be a consideration for real-time predictions.

## Conclusion

This project demonstrates the application of supervised learning algorithms to predict mushroom edibility. The k-NN model showed superior performance compared to Logistic Regression. However, the choice of the model should consider the specific application requirements, including accuracy, computational efficiency, and the nature of the data.

## How to Run

1. Clone the repository from GitHub.
2. Navigate to the project directory.
3. Install the required libraries by referring to `requirements.txt`.
4. Open the Jupyter Notebook and run the cells to see the implementation.

## Acknowledgments

- The authors of "Introduction to Machine Learning with Python"
- scikit-learn documentation and community
- [@prishasawhney](https://www.kaggle.com/prishasawhney) from Kaggle for providing the dataset
