# SCT_DS_Task03
 public repository to showcase my data science tasks from my internship, including a decision tree classifier on the Bank Marketing dataset

# Bank Marketing Campaign Analysis: A Decision Tree Classifier
This project aims to build a predictive model using a **Decision Tree Classifier** to determine whether a bank customer will subscribe to a term deposit. The analysis uses the **Bank Marketing Dataset** from the UCI Machine Learning Repository, which contains data from direct marketing campaigns.
A key focus of this project was to handle the challenge of an **imbalanced dataset** and evaluate the model's performance beyond simple accuracy. The analysis includes detailed visualizations of feature distributions and a deep dive into the **Confusion Matrix** to derive actionable business insights.


**Methodology**

i) Data Loading and Initial Exploration: Loaded the bank-full.csv dataset and performed initial checks.

ii) Data Preprocessing:
--> Encoded the categorical features (e.g., job, marital) using One-Hot Encoding to prepare the data for the model.

--> Converted the target variable y ('yes'/'no') into numerical labels (0/1) using a Label Encoder.

--> Split the data into a training set and a testing set (80/20 split) to ensure robust model evaluation.

iii)Model Training: A DecisionTreeClassifier was trained using the preprocessed training data.

iv) Model Evaluation: The model was evaluated on the test set using key metrics, including:
--> Confusion Matrix: To analyze True Positives, True Negatives, False Positives, and False Negatives.

--> Classification Report: To assess Precision, Recall, and F1-Score, which are more reliable for imbalanced datasets than accuracy alone.

**Key Findings and Results**

i) The model achieved an overall accuracy of 91%. However, a closer look at the confusion matrix and classification report revealed a more nuanced picture, which is critical for business strategy:

ii) High True Negative Rate: The model was highly effective at correctly identifying customers who would not subscribe, which helps in efficient resource allocation.

iii) Low Recall for the Positive Class: The model's recall for predicting yes was approximately 44%. This means a significant number of actual subscribers were missed, representing a potential loss of revenue.

iv) Visual Insights: Exploratory data analysis showed that age and marital status have a strong correlation with subscription rates, providing valuable insights for future targeted campaigns.

**Tools and Libraries**

i) Python: The core programming language.

ii) Pandas: For data manipulation and analysis.

iii) Scikit-learn: For machine learning tasks, including preprocessing (OneHotEncoder), model building (DecisionTreeClassifier), and evaluation (confusion_matrix, classification_report).

iv) Matplotlib & Seaborn: For data visualization and plotting the confusion matrix and feature distributions.
