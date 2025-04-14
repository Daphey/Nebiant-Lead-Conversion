# Nebiant-Lead-Conversion

### Introduction
In this analysis, the objective is to develop a Predictive Lead Scoring model designed to prioritize leads based on their likelihood of conversion. This model aims to provide Nebiant Analytics team with actionable insights, enabling them to focus their efforts on high-value leads that are more likely to convert.

The core goal is to create a model that predicts the probability of lead conversion, classifying leads into categories such as "High", "Medium", or "Low" probability. By accurately identifying the most promising leads, the model will help optimize resource allocation and improve the efficiency of the sales process.

The impact of this analysis is significant as it allows the sales team to focus on the leads with the highest potential, ultimately increasing conversion rates and driving business growth.


### Steps Taken to Build the Model

- **Data Preprocessing**
  - Addressed missing values
  - Managed outliers
  - Checked for duplicates
  
- **Exploratory Data Analysis (EDA)**
  - Analyzed the data to uncover and understand patterns

- **Feature Engineering**
   - Encoded categorical features
   - Created a Time-to-Start column
   - Analyzed the sentiment of texts, then created Sentiment Category and Sentiment Score columns
   - Applied TF-IDF to convert text data into numerical features
   - Used K-Means clustering to group similar texts and added the resulting cluster labels as a new feature

- **Model Training**
   - Selected label and feature variables
   - Applied Supervised Learning: Trained classifiers (Logistic Regression, Random Forest, Decision Tree) using the engineered features
   - Hyperparameter Tuning: Optimized model parameters using GridSearchCV or RandomizedSearchCV

- **Model Evaluation**
   - Performed Train-Test Split: Split the dataset into training and testing sets
   - Calculated model accuracy on both training and testing data
   - Assessed model performance using metrics such as accuracy, precision, recall, and F1-score
   
- **Predictive Scoring for All Classes**
Generated predictive scores for each sentiment class

- **Feature Importance Analysis**
Used SHAP (Shapley Additive Explanations) to assess feature importance

- **Conclusion and Observations**
Summarized key findings and noted areas for improvement
