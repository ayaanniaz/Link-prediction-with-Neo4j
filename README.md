# Link-prediction-with-Neo4j
Link Prediction on Facebook Food Pages Network using Neo4j & Supervised ML

This project predicts future mutual likes (links) between Facebook pages of food joints, restaurants, and celebrity chefs. Using Neo4j Graph Data Science (GDS) and supervised machine learning, the model identifies potential new connections based on graph structural features.

# Project Overview

Build a graph of Facebook food pages (nodes) and mutual likes (edges)

Generate link prediction features using GDS similarity algorithms

Create labeled dataset (positive = existing links, negative = non-links)

Train a Random Forest classifier for supervised link prediction

Evaluate using ROC-AUC, confusion matrix, and feature importance

Predict top potential future connections between pages

Visualize ego networks using NetworkX

# Dataset

Source: https://networkrepository.com/
Dataset: fb-pages-food.zip
Contains:

Nodes: Facebook pages of food joints & chefs

Edges: Mutual page likes (undirected)

# Tech Stack

Neo4j + Graph Data Science (GDS)

Python (Neo4j driver, Pandas, NumPy, scikit-learn)

NetworkX & Matplotlib for visualization

# Methodology

Import nodes & edges into Neo4j

Compute link prediction features:

Common Neighbors

Adamic-Adar

Preferential Attachment

Build positive & negative training samples

Train a Random Forest classifier

Predict new potential links

Visualize ego networks with predicted connections

# Results

ROC-AUC: ~0.92

Adamic-Adar was the most important feature

Model successfully identified high-probability future connections

Ego network visualization highlights predicted relationships
