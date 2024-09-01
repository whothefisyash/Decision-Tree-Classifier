# Decision Tree Classifier
This project demonstrates the implementation of a Decision Tree Classifier using Scikit-learn and visualizes the decision boundary and the tree structure. The classifier is applied to a synthetic dataset to illustrate its performance and characteristics.

## Overview
The Decision Tree Classifier is a supervised learning algorithm that is used for both classification and regression tasks. It works by splitting the dataset into subsets based on the most significant attribute, creating a tree-like structure where each internal node represents a decision on an attribute, and each leaf node represents the outcome.

## This project includes:

Training a Decision Tree Classifier on a synthetic dataset generated using make_moons.
Visualizing the decision boundary of the trained classifier.
Visualizing the structure of the decision tree.
Allowing customization of various hyperparameters through a web interface built with Streamlit.
Features
Interactive Web Interface: Users can interactively adjust the hyperparameters of the Decision Tree, such as criterion, max_depth, min_samples_split, min_samples_leaf, and more.
Decision Boundary Visualization: The decision boundary created by the classifier is plotted, showing how the model classifies different regions of the input space.
Tree Structure Visualization: The structure of the trained Decision Tree is visualized, displaying the splits made at each node.
Accuracy Metric: The accuracy of the model on the test set is displayed after training.
Usage
Data Generation: The dataset used in this project is generated using the make_moons function from Scikit-learn, which creates a two-class dataset with a non-linear decision boundary.

Model Training: The model is trained on the generated dataset using the DecisionTreeClassifier from Scikit-learn.

Parameter Tuning: Users can adjust the following parameters:

criterion: The function to measure the quality of a split. Options include "gini" for the Gini impurity and "entropy" for information gain.
max_depth: The maximum depth of the tree. If set to None, nodes are expanded until all leaves are pure.
min_samples_split: The minimum number of samples required to split an internal node.
min_samples_leaf: The minimum number of samples required to be at a leaf node.
max_features: The number of features to consider when looking for the best split.
max_leaf_nodes: The maximum number of leaf nodes.
min_impurity_decrease: A node will be split if this split induces a decrease in the impurity greater than or equal to this value.
Visualization:

Decision Boundary: The decision boundary is visualized using a contour plot, which shows how the classifier partitions the feature space.
Decision Tree: The structure of the trained Decision Tree is visualized using the dtreeviz library, which provides a detailed and interpretable tree diagram.
Running the Application: The application is run using Streamlit, providing an interactive and user-friendly interface.

Code Structure
app.py: The main application file that includes the implementation of the Decision Tree Classifier, the Streamlit interface, and the visualization logic.
assets/: This directory contains any assets used by the application, such as images or additional data files (if any).
README.md: This file, which provides an overview of the project, features, and usage instructions.
