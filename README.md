# house-price-prediction

Regression

Dataset used comes from UCI Machine Learning
Includes 14 features of homes from various suburbs located in Boston

Using XGBoost.

XGBoost, which stands for eXtreme Gradient Boosting, is a powerful and widely used machine learning algorithm that belongs to the class of gradient boosting algorithms. It has gained popularity in various machine learning competitions due to its effectiveness in handling a wide range of data types and producing highly accurate models. Here's an explanation of what XGBoost is and how it works:

What is XGBoost?
XGBoost is an implementation of gradient boosting designed for speed and performance. Gradient boosting is an ensemble learning technique where multiple weak learners (typically decision trees) are trained sequentially, with each tree correcting the errors of its predecessor. XGBoost extends traditional gradient boosting by introducing some key innovations to improve both speed and model performance.

Key Features of XGBoost:
Regularization: XGBoost incorporates L1 (LASSO) and L2 (ridge) regularization terms into the objective function. This helps prevent overfitting and makes the algorithm more robust.

Parallelization: XGBoost is designed to be highly parallelizable, making it efficient for training on large datasets.

Handling Missing Values: XGBoost can handle missing values in the dataset, assigning appropriate default directions in decision trees for instances with missing values.

Tree Pruning: The algorithm uses a depth-first approach during tree construction and prunes branches that contribute little to the overall reduction in the loss function. This helps to control the complexity of the model and avoid overfitting.

Cross-validation: XGBoost supports built-in cross-validation during the training process, allowing for more robust model evaluation.

How XGBoost Works:
Initialize with a Simple Model: The algorithm starts with a simple model, usually a single leaf, representing the mean of the target variable.

Calculate Residuals: The residuals (differences between actual and predicted values) are computed for each instance.

Train a Weak Learner (Decision Tree): A decision tree is trained to predict the negative gradient (residuals) of the loss function. The tree is added to the ensemble.

Update Predictions: The predictions are updated by adding the predictions of the new tree, and this process is repeated for a specified number of iterations or until a stopping criterion is met.

Regularization and Pruning: Regularization terms and pruning techniques are applied during the tree construction to control the complexity of the model and prevent overfitting.

Final Prediction: The final prediction is the sum of the initial model's prediction and the predictions from all subsequent trees.

Usage of XGBoost:
XGBoost is versatile and can be used for both classification and regression tasks. Some common applications and use cases include:

Predictive Modeling: XGBoost is widely used for predictive modeling in various domains such as finance, healthcare, and marketing.

Feature Importance Analysis: XGBoost provides a way to assess the importance of different features in the dataset, aiding in feature selection.

Anomaly Detection: XGBoost can be used for anomaly detection by identifying instances that deviate significantly from the expected pattern.

Ranking Problems: XGBoost can be applied to ranking problems, such as search engine result ranking.

Time Series Forecasting: XGBoost can be adapted for time series forecasting, leveraging its ability to capture complex patterns.

When using XGBoost, it's important to fine-tune hyperparameters, perform feature engineering, and carefully validate the model to achieve optimal performance. The algorithm has become a go-to choice in many machine learning projects due to its robustness, efficiency, and ability to handle diverse data types.