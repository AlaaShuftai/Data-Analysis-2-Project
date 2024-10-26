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

NLTK (Natural Language Toolkit): A suite of libraries for natural language processing, such as tokenization, stemming, and sentiment analysis.

Orange: A visual programming and machine learning toolkit for data mining and visualization, especially for non-coders.

MLxtend: Provides additional tools and extensions for Scikit-Learn, including association rule mining and data analysis tools.

Statsmodels: A library for estimating and testing statistical models, with tools for performing hypothesis tests and regression analysis.

Pyplot: A Matplotlib module that provides a MATLAB-like interface for creating various types of plots and charts.


### Conclusion:
Survival on the Titanic dataset, with key features like Embarked and Sex being pivotal in determining survival likelihood. The evaluation metrics provided a comprehensive balance of accuracy, precision, and recall. Future improvements could involve experimenting with different algorithms or more advanced feature  techniques.
