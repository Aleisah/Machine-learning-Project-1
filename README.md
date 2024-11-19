# Classification of Forest Cover Type

Objective:
The aim of this project is to build a machine learning pipeline that classifies forest
cover types based on cartographic features such as elevation, soil type, and
climatic conditions. The project will include a comparison of various classification
algorithms and their performance.

Dataset:
The dataset used in this project is the Forest Cover Type dataset available on
https://www.kaggle.com/datasets/uciml/forest-cover-type-dataset.
The dataset contains 54 features, including ~40 binary columns representing
different soil types. The target variable is the forest cover type, which has 7
distinct classes.

## Steps Followed
1. **Data Loading:**
   - Downloaded the dataset from Kaggle.
   - Loaded using Pandas and inspected for structure, feature types, and missing values.

2. **Data Preprocessing:**
   - Handled missing data (if any).
   - Performed feature engineering to drop irrelevant columns and create new features.
   - Ensured proper encoding of categorical variables (one-hot encoding for soil types).

3. **Feature Scaling:**
   - No Scaling: The raw data was used as-is without applying any scaling.
   - MinMaxScaler: Scales the data to a range of [0, 1].
   - StandardScaler: Standardizes features by removing the mean and scaling to unit variance.

4. **balancing the data**
   - transforms features to make their distributions more Gaussian-like.
   - Under-sampling reduces the number of samples in the majority class to match the minority class.

5. **Data Splitting:**
   - Split the data into training and testing sets.
   - Conducted correlation analysis and feature selection.

6. **Classification Algorithms Applied:**
   - Logistic Regression
   - Decision Trees
   - Random Forest
   - k-Nearest Neighbors (k-NN)

   Models were trained on the training set and evaluated on the test set using:
   - Accuracy
   - Precision
   - Recall
   - F1-score
     
8. **Comparison of Results:**
   - Analyzed the models based on performance metrics.
   - Identified the best-performing algorithm.

## Dependencies
The project requires the following Python libraries:
- `pandas`
- `numpy`
- `plotly`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `imblearn`

To install all dependencies:
```bash
pip install -r requirements.txt
```

Mohammad Aleisah
Wish You The Best
