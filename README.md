## Zoo Animal Classifier

A small supervised ML project that classifies zoo animals into seven groups (Mammals, Birds, Reptiles, Fish, Amphibians, Bugs, Invertebrates) using a K-Nearest Neighbors classifier.

Project by Jomana Shaltout — DecodeLabs Project 2

#### Summary

This demonstrates an end-to-end machine learning workflow on the Zoo Animal Classification dataset (101 animals, 16 features). The pipeline covers data loading, basic exploration, preprocessing (scaling), training a KNN classifier, evaluation (confusion matrix, F1-score), and visualization.

#### Dataset

Source: Zoo Animal Classification (UCI / Kaggle).

Files: zoo.csv (features) and class.csv (labels) — included in the repo or linked.

Features include: animal_name, hair, feathers, eggs, milk, airborne, aquatic, predator, toothed, backbone, breathes, venomous, fins, tail, domestic, legs, class_type.

Size: 101 samples across 7 classes.

#### How it works

Load and inspect data (shape, data types, class distribution).

Prepare features and labels, drop non-predictive columns (e.g., animal_name).

Split data: 80% train / 20% test, shuffled and stratified.

Scale numeric features with StandardScaler to normalize ranges for KNN.

Train KNeighborsClassifier and predict on test set.

Evaluate using confusion matrix and F1-score.

Visualize class distribution and confusion matrix.

#### Results and visuals

Class distribution bar chart (counts per class).

Confusion matrix heatmap comparing true vs predicted labels.

Reported metrics: accuracy and macro F1. In this project’s run, only one test sample was misclassified.

#### Limitations

Small dataset (101 samples) — limited generalization.

Some features (e.g., catsize) need clarification or cleaning.

No model comparison or hyperparameter tuning beyond basic setup.

#### Recommended improvements

Compare KNN to other classifiers.

Clean ambiguous features and clearly document feature meanings.

#### References

Dataset: https://www.kaggle.com/datasets/uciml/zoo-animal-classification/data

