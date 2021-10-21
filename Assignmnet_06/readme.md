**Diabetes Classification using Logistic Regression and it's evaluation metrics**

**Objectives**: To develop a machine learning model to predict diabetes using the input features and calculate its performance by 'recall' metric. To analyze the model using liblinear & lbfgs solvers at various regularization strengths with grid cross-validation of 10 folds.

**Conclusions:**

1) Here, we have choosen Recall as our evalution metric, as we are concerned about false negatives.

2) The Recall for the base Logistic Regression Model is 51%, so the model needs hyper parameter tuning to achieve better recall value. so we can say that the 51% of the diabetic class is correctly predicted.

3) After 10 fold cross-validation and having L2 regularization strength with liblinear solver, the model performned better with the recall score of 76.54%

4) Logistic Regression with l2 regularization and liblinear solver is the best model as it increased the recall by decreasing the false negatives.

5) The lbfgs solver has not increased the recall score as compared with the liblinear solver. Thus, Logistic Regression with l2 regularization and liblinear solver is the best model to predict the presence of diabetis.

6) Reducing the value of C, improved the performnace of the model.

7) Grid Search Cross-Validation has improved the model's performance.
