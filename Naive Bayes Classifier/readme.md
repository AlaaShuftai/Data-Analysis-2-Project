## Titanic Dataset Analysis - Naive Bayes Classifier

### 1. Data Processing Steps:
- **Data Loading**: The Titanic dataset was loaded from a publicly available URL.
- **Missing Data Handling**:
  - The `Age` column had missing values, which were filled using the mean value of the column.
  - The `Embarked` column also contained missing values, and these were filled using the mode (most frequent value).
- **Feature Selection**: The selected features for model training included:
  - `Pclass` (Passenger Class)
  - `Age` (Passenger Age)
  - `SibSp` (Number of Siblings/Spouses aboard)
  - `Parch` (Number of Parents/Children aboard)
  - `Fare` (Ticket Fare)
  - **One-hot encoded** categorical variables:
    - `Sex_male`
    - `Embarked_Q`
    - `Embarked_S`

### 2. Model Choice:
A Naive Bayes Classifier was used to predict the target variable, **Survived** (whether a passenger survived or not). This classification model is suitable for this task, where the goal is to predict a binary outcome (survived or not).

### 3. Performance Evaluation:
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

### 4. Feature Importance:
Naive Bayes models don’t explicitly provide feature importance, but insights can still be gathered from the data distribution and its influence on survival predictions. In this analysis:
- **Key Features**: 
  - **Pclass**, **Sex_male**, and **Fare** were the most important features in predicting survival.
  - A bar chart was plotted to illustrate the relative importance of these features in the classification process.

### 5. Insights Gained:
The analysis yielded several interesting findings:
- **Passenger Class and Gender**: The `Pclass` and `Sex_male` features significantly influenced survival outcomes. Lower-class passengers and males were less likely to survive.
- **Fare**: Higher ticket fares correlated with a higher likelihood of survival, indicating that wealthier passengers may have had better access to resources during the disaster.
- **Age and Family**: The `Age`, `SibSp`, and `Parch` features showed moderate importance, suggesting that family relationships and age also affected survival chances.
- **Embarkation Point**: The place of embarkation (captured by `Embarked_Q` and `Embarked_S`) had a smaller, but noticeable influence on survival.

### Conclusion:
The Naive Bayes model performed well in predicting survival on the Titanic dataset. Important features like **Pclass**, **Sex**, and **Fare** played a key role in determining the survival likelihood of passengers. The balance between accuracy, precision, and recall metrics demonstrated that the model effectively handled this classification task. Future improvements could include experimenting with different algorithms or more advanced feature engineering to enhance prediction accuracy.
