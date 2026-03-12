# Iris k-NN Classifier

This project implements a **k-Nearest Neighbors (k-NN) classifier** to predict the species of iris flowers using the classic Iris dataset.  
The notebook demonstrates data preprocessing, training, evaluation, and displaying correct and wrong predictions.

---

## Dataset

The Iris dataset contains **150 samples** with the following features:

- Sepal length (cm)
- Sepal width (cm)
- Petal length (cm)
- Petal width (cm)

The target variable is the **species of the iris**:

- Setosa
- Versicolor
- Virginica

---

## Steps Performed

1. **Load Dataset**
   - Load Iris dataset using `sklearn.datasets.load_iris()`
   - Convert to Pandas DataFrame for inspection

2. **Train-Test Split**
   - Split data into **70% training** and **30% testing** using `train_test_split`

3. **Feature Scaling**
   - Standardize features using `StandardScaler` for improved k-NN performance

4. **Model Training**
   - Initialize k-NN classifier with `k=5` neighbors
   - Fit the model on scaled training data

5. **Prediction and Evaluation**
   - Predict iris species for test set
   - Calculate **accuracy** using `accuracy_score`
   - Display correct and wrong predictions

---

## Results

- Training samples: 105  
- Testing samples: 45  
- **k-NN Accuracy:** 100%  

**Correct Predictions Example:**

| Features                  | Actual Species | Predicted Species |
|----------------------------|----------------|-----------------|
| [6.1, 2.8, 4.7, 1.2]      | Versicolor     | Versicolor      |
| [5.7, 3.8, 1.7, 0.3]      | Setosa         | Setosa          |
| [7.7, 2.6, 6.9, 2.3]      | Virginica      | Virginica       |

**Wrong Predictions:**  
- None in this run (100% accuracy)
git clone https://github.com/<username>/iris-knn-classifier.git

