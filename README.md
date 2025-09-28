# Adaline Implementation on Iris Dataset

This project contains the implementation of the **Adaline (Adaptive Linear Neuron)** model from scratch and its application to a subset of the **Iris dataset** for binary classification. The work was done as part of the *Neural Networks and Deep Learning* course homework.

## 📌 Project Description

The goal of this project is to:

* Understand the **Adaline** and **Madaline** algorithms as early neural network models.
* Implement the Adaline learning algorithm in Python.
* Train and evaluate the model on a binary classification task using the **Iris dataset (Setosa vs. Versicolor)**.
* Compare the effect of different learning rates.
* Visualize and analyze the results.

## ⚙️ Tasks Overview

### 1. Theory & Background

* Explained **Adaline** and **Madaline** algorithms.
* Highlighted differences between **Madaline** and **MLP**.

### 2. Data Preparation

* Loaded Iris dataset using `sklearn.datasets.load_iris`.
* Selected only two classes: **Setosa** and **Versicolor**.
* Used features: **petal length** and **petal width**.
* Normalized data into range `[0, 1]`.
* Split into **70% training** and **30% testing**.

### 3. Adaline Implementation

* Implemented Adaline model with:

  * Input/output dimensions.
  * Learning rate.
  * Number of epochs.
* Recorded:

  * Weights and biases per epoch.
  * Error per epoch.
  * Training accuracy per epoch.

### 4. Training & Evaluation

* Trained Adaline with **3 learning rates**: `0.02`, `0.005`, `0.001`.
* Each model trained for **10 epochs**.
* Stored error and accuracy per epoch.

### 5. Results & Visualization

* Plotted **decision boundaries** for training and testing sets.
* Plotted **error vs. epochs** and **accuracy vs. epochs** for each learning rate.
* Analyzed:

  * Convergence behavior of different learning rates.
  * Effect of linear separability on Adaline’s performance.
  * Comparison of training vs. testing performance.

## 📊 Example Results

* Higher learning rates converge faster but may oscillate.
* Very small learning rates lead to slow convergence.
* Since the two chosen classes are **linearly separable**, Adaline performs well.
* For non-linearly separable data, Adaline fails to generalize effectively.

## 🧠 Key Takeaways

* Adaline demonstrates the role of **linear classifiers** in early neural network models.
* Learning rate is crucial: too high → unstable, too low → slow convergence.
* Works well only when data is **linearly separable**.
