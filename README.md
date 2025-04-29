# logistic-regression
Objective:
We built a binary classifier using logistic regression to classify whether a tumor is malignant (0) or benign (1) using the Breast Cancer Wisconsin dataset.

Step-by-Step explanation
Step 1: Import Libraries
We import all necessary libraries:

pandas, numpy for data handling.

scikit-learn tools for preprocessing, model training, and evaluation.

matplotlib, seaborn for visualization.

Step 2: Load Dataset
We use the built-in load_breast_cancer() dataset from scikit-learn:

X: features (like cell size, shape, etc.)

y: target labels (0 = malignant, 1 = benign)

Step 3: Train-Test Split
We split the dataset:

80% for training

20% for testing
This helps us evaluate how well the model performs on unseen data.

Step 4: Feature Scaling
We standardize the features using StandardScaler:

Logistic regression is sensitive to scale.

Standardization transforms features to have mean = 0 and std = 1.

Step 5: Train Model
We fit a Logistic Regression model on the training data.

Step 6: Predictions
y_pred: Predicted class labels (0 or 1)

y_prob: Predicted probabilities (needed for ROC-AUC curve)

Step 7: Evaluation Metrics
We calculate:

Confusion Matrix: Tells us TP, FP, TN, FN.

Precision: How many predicted positives are actually positive.

Recall: How many actual positives are correctly predicted.

ROC-AUC: Measures how well the model separates the classes.

Step 8: Plot Confusion Matrix
We visualize the confusion matrix using a heatmap to understand misclassifications.

Step 9: Plot ROC Curve
We plot TPR vs FPR using predicted probabilities.

The closer the curve is to top-left, the better.

AUC value close to 1 indicates a strong model.

Step 10: Sigmoid Function
We visualize the sigmoid function, which maps any real number to a probability between 0 and 1:

𝜎(𝑧)=1/1+𝑒^−𝑧

​
 
This is the core of logistic regression.

