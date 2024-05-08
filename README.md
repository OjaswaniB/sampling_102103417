# Sampling
Sampling is the process of selecting a subset of elements from a larger population to represent and analyze, often used in research or statistics to draw conclusions about the entire group based on the sampled data.

![image](https://github.com/nitleenk/Sampling/assets/127779292/52776dd3-4874-4224-a50e-4e0d563468f4)

Dataset
The dataset used in this project is available in Creditcard_data.csv. It contains the following columns:

1. Time: Number of seconds elapsed between this transaction and the first transaction in the dataset.
2. V1-V28: Principal components obtained with PCA, anonymized features.
3. Amount: Transaction amount.
4. Class: Target variable indicating whether the transaction is fraudulent (1) or not (0).

Sampling Techniques Used
1. RandomUnderSampler :A method that randomly removes instances from the majority class to balance class distribution in imbalanced datasets.
2. RandomOverSampler :A technique that randomly duplicates instances from the minority class to balance class distribution in imbalanced datasets.
3. SMOTE (Synthetic Minority Over-sampling Technique) :A method that generates synthetic samples in the minority class by interpolating between existing instances to address class imbalance.
4. BorderlineSMOTE :A variation of SMOTE that focuses on generating synthetic samples near the borderline between classes to address imbalanced datasets.
5. ADASYN (Adaptive Synthetic Sampling) :A technique similar to SMOTE but adjusts the sampling density based on the level of difficulty of learning areas to generate more informative synthetic samples.

Classifier Used
1. LogisticRegression :A linear model used for classification that predicts the probability of an instance belonging to a particular class.
2. DecisionTreeClassifier :A non-parametric model that makes decisions based on a tree-like structure, learning simple decision rules inferred from the data features.
3. RandomForestClassifier :An ensemble learning method that constructs multiple decision trees during training and outputs the class that is the mode of the classes of the individual trees.
4. SVC (Support Vector Classifier) :A classifier that finds the hyperplane that best separates classes in a high-dimensional space by maximizing the margin between classes.
5. GradientBoostingClassifier : A boosting ensemble method that builds a strong classifier by combining multiple weak classifiers in a stage-wise manner, minimizing the loss function's gradient.
