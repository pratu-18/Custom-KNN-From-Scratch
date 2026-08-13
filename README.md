# Custom-KNN-From-Scratch
# KNN From Scratch in Python

A simple implementation of the **K-Nearest Neighbors (KNN) classification algorithm from scratch using Python**, without using the built-in KNN classifier from Scikit-learn.

## Project Overview

This project demonstrates how the KNN algorithm works internally by implementing its main steps manually:

- Euclidean distance calculation
- Distance calculation between points
- Sorting points based on distance
- Selecting K nearest neighbours
- Majority voting
- Final class prediction

## Case Study

In this case study, each data point represents a point in a 2D coordinate system with:

- X coordinate
- Y coordinate
- Class label

The dataset contains two classes:

- Red
- Blue

A new point is provided to the classifier, and the algorithm determines whether the new point belongs to the **Red** or **Blue** class.

## Example

New point:

```text
X = 3
Y = 3
