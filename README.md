Task 5: Decision Trees and Random Forests

About this Task:

-Hey! This is my fifth task where I worked with tree-based models for classification using the Heart Disease dataset (heart.csv).

-The goal was to predict if a person has heart disease (target = 1) or not (target = 0) based on different medical attributes.

What I did in this task:
1.Loaded the Heart Disease dataset using Pandas from a CSV file (heart.csv).

2.Split the dataset into features and target.

i.Target = 1 (Disease), 0 (No Disease)

ii.Features included Age, Cholesterol, Blood Pressure, etc.

3.Split the data into train and test sets (80% for training and 20% for testing).

4.Trained a Decision Tree Classifier on the training data.

5.Evaluated the Decision Tree’s accuracy on the test data → It gave very high accuracy (~98.5%) (but I knew it could be overfitting).

6.Visualized the Decision Tree (first 3 levels) using Matplotlib.
-The plot showed feature splits, Gini values, and class labels.

7.Controlled overfitting by limiting tree depth (Pruning)

i.Set max_depth=4 and retrained the Decision Tree

ii.Test accuracy dropped to ~80%, showing the trade-off between complexity and generalization.

8.Trained a Random Forest Classifier with 100 trees.

i.The accuracy improved again to around 98.5%

ii.Random Forest reduced overfitting while maintaining high accuracy.

9.Compared accuracies between:

i.Full Decision Tree

ii.Pruned Decision Tree

iii.Random Forest

10.Checked feature importances from Random Forest

i.Found that features like cp, ca, thalach, and oldpeak were most important for predicting heart disease.

11.Evaluated Random Forest using 5-Fold Cross-Validation

i.Got very high and stable CV scores (~99.7% mean accuracy)

ii.This showed that the Random Forest generalizes well.

