# Linear vs Non-Linear Classification with PyTorch

This project demonstrates the difference between linear and non-linear classification using Artificial Neural Networks (ANNs) built with PyTorch.

Two datasets are used:

1. Email Classification Dataset (Linearly Separable)
2. Seismic Activity Dataset (Non-Linearly Separable)

The objective is to compare how a simple linear neural network and a neural network with ReLU activation perform on different data structures.

---

## Project Goals

- Understand binary classification
- Learn the difference between linear and non-linear decision boundaries
- Build neural networks using PyTorch
- Visualize classification results
- Compare model performance on different datasets

---

## Dataset 1: Email Classification

Features:

- subject_formality_score
- sender_relationship_score

Target:

- 0 = Personal Email
- 1 = Work Email

This dataset is linearly separable and can be classified successfully using a simple linear neural network.

---

## Dataset 2: Seismic Activity Classification

Features:

- underground_wave_energy
- vibration_axis_variation

Target:

- 0 = No Seismic Event
- 1 = Seismic Event Detected

This dataset contains non-linear patterns and requires hidden layers with activation functions to achieve high accuracy.

---

## Models

### Linear Model

Architecture:

```text
2 → 5 → 1
```

No activation function is used.

Suitable for linearly separable data.

### Non-Linear Model

Architecture:

```text
2 → 10 → 10 → 1
```

Activation Function:

```text
ReLU
```

Suitable for non-linearly separable data.

---

## Results

### Email Dataset

Linear model achieved high accuracy because the classes can be separated by a straight line.

### Seismic Dataset

Linear model struggled to classify the data.

The non-linear model successfully learned the complex decision boundary and achieved near-perfect accuracy.

---

## Technologies

- Python
- PyTorch
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-Learn

---

## Learning Outcomes

This project demonstrates why activation functions are essential in neural networks and how non-linear models can solve problems that linear models cannot.

---

## Disclaimer

This project was developed as part of a neural networks learning exercise. The datasets and overall workflow were provided during coursework and adapted for educational purposes.
