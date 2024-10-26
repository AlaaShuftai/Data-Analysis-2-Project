## Titanic Dataset Analysis - Naive Bayes Classifier

### Short description:
In this task, we implemented the Naive Bayes classifier using Scikit-Learn to categorize data based on probabilistic reasoning. After preprocessing the data, we split it into training and testing sets. We then initialized the Naive Bayes model (e.g., GaussianNB for continuous data) and trained it on the training set. Finally, we evaluated the model’s performance on the test set using accuracy and other relevant metrics to assess its classification effectiveness.

Titanic Dataset (https://www.kaggle.com/c/titanic/data)


### Model Choice:
A Naive Bayes Classifier was used to predict the target variable, **Survived** (whether a passenger survived or not). This classification model is suitable for this task, where the goal is to predict a binary outcome (survived or not).


### libraries we used:

NumPy: A library for numerical computations in Python, especially for handling arrays and performing mathematical operations.

Pandas: A data manipulation and analysis library that provides data structures (DataFrames) for efficiently handling large datasets.

Scikit-Learn: A machine learning library providing tools for data preprocessing, classification, regression, clustering, and model evaluation.

Matplotlib: A plotting library for creating static, interactive, and animated visualizations in Python.

Seaborn: Built on Matplotlib, this library offers a high-level interface for drawing statistical graphics.

Pyplot: A Matplotlib module that provides a MATLAB-like interface for creating various types of plots and charts.


### Conclusion:
This project implemented a naive Bayes classifier using Scikit-Learn to classify data based on probabilistic principles. After preprocessing, the dataset was split into training and test sets. A Gaussian naive Bayes model was trained on the training data and evaluated on the test data using accuracy and other metrics. Insights from the final graphs suggest that the port of embarkation significantly affects survival predictions, possibly due to the order of embarkation or many other factors.
