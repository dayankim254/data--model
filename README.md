This program is designed to help predict which students are likely to enroll in a program and which students may need additional support to graduate. It uses a dataset containing student details like their GPA, Age, Gender, and two key outcomes: Enrollment_Status (whether the student enrolled) and Graduation_Status (whether the student graduated).

Here’s how the code works step by step:

Loading the Data:

The program begins by importing a CSV file with historical student data. This dataset includes academic records, demographics, and the outcomes we aim to predict.
Selecting Features and Targets:

It identifies the input features (GPA, Age, Gender) and defines two separate target variables:
Enrollment_Status: Helps determine whether a student will enroll in the program.
Graduation_Status: Predicts if a student will successfully complete the program.
Enrollment Prediction:

The dataset is split into training and testing subsets, ensuring the model can be evaluated on unseen data.
A logistic regression model is trained using the selected features to predict enrollment.
The model's performance is evaluated through:
A confusion matrix, which shows the counts of correct and incorrect predictions.
A classification report, summarizing precision, recall, F1-score, and overall accuracy.
To visualize the model's ability to distinguish between students who enroll and those who don’t, an ROC curve is plotted. The curve compares the true positive rate (students correctly predicted to enroll) to the false positive rate.
Graduation Prediction:

A similar process is repeated to predict whether a student will graduate:
The data is divided into training and testing sets.
Features are normalized for consistency.
A logistic regression model is trained specifically for graduation prediction.
The evaluation includes the same metrics (confusion matrix and classification report).
Another ROC curve is plotted, showing the model's performance in predicting graduation outcomes.
Visualizing Performance:

The program generates two separate ROC curves:
Enrollment ROC Curve: Visualizes the model's performance for predicting student enrollment.
Graduation ROC Curve: Displays the accuracy of predictions for graduation success.
These curves provide a clear and intuitive way to understand the effectiveness of the models.
