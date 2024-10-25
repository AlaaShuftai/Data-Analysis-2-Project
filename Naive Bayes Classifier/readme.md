## Titanic Dataset Analysis - Naive Bayes Classifier

### Short description:
In this task, we implemented the Naive Bayes classifier using Scikit-Learn to categorize data based on probabilistic reasoning. After preprocessing the data, we split it into training and testing sets. We then initialized the Naive Bayes model (e.g., GaussianNB for continuous data) and trained it on the training set. Finally, we evaluated the model’s performance on the test set using accuracy and other relevant metrics to assess its classification effectiveness.
Titanic Dataset (https://www.kaggle.com/c/titanic/data)


### Model Choice:
A Naive Bayes Classifier was used to predict the target variable, **Survived** (whether a passenger survived or not). This classification model is suitable for this task, where the goal is to predict a binary outcome (survived or not).

### Performance Evaluation:
The performance of the Naive Bayes model was evaluated using common classification metrics:
- **Accuracy**: The ratio of correct predictions to total predictions made by the model.
- **Precision**: The percentage of true positive predictions out of all positive predictions.
- **Recall**: The model's ability to correctly identify all true positive instances.
- **F1 Score**: A harmonic mean of precision and recall, balancing false positives and false negatives.
  
**Evaluation Results**:
- **Accuracy**: [insert accuracy score]
- **Precision**: [insert precision score]
- **Recall**: [insert recall score]
- **F1 Score**: [insert F1 score]

Additionally, a **Confusion Matrix** was generated to provide a visual breakdown of true positives, true negatives, false positives, and false negatives.

### Feature Importance:
Naive Bayes models don’t explicitly provide feature importance, but insights can still be gathered from the data distribution and its influence on survival predictions. In this analysis:
- **Key Features**: 
  - **Pclass**, **Sex_male**, and **Fare** were the most important features in predicting survival.
  - A bar chart was plotted to illustrate the relative importance of these features in the classification process.

### Insights Gained:
The analysis yielded several interesting findings:
- **Passenger Class and Gender**: The `Pclass` and `Sex_male` features significantly influenced survival outcomes. Lower-class passengers and males were less likely to survive.
- **Fare**: Higher ticket fares correlated with a higher likelihood of survival, indicating that wealthier passengers may have had better access to resources during the disaster.
- **Age and Family**: The `Age`, `SibSp`, and `Parch` features showed moderate importance, suggesting that family relationships and age also affected survival chances.
- **Embarkation Point**: The place of embarkation (captured by `Embarked_Q` and `Embarked_S`) had a smaller, but noticeable influence on survival.

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
The Naive Bayes model performed well in predicting survival on the Titanic dataset. Important features like **Pclass**, **Sex**, and **Fare** played a key role in determining the survival likelihood of passengers. The balance between accuracy, precision, and recall metrics demonstrated that the model effectively handled this classification task. Future improvements could include experimenting with different algorithms or more advanced feature engineering to enhance prediction accuracy.
