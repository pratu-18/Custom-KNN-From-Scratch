# KNN CLASSIFIER FROM SCRATCH

1. PROJECT DESCRIPTION

---

This project demonstrates a custom implementation of the K-Nearest Neighbors
(KNN) classification algorithm using Python.

The KNN algorithm is implemented completely from scratch without using the
built-in KNN classifier provided by machine learning libraries such as
Scikit-learn.

The project uses Euclidean Distance to calculate the distance between data
points and majority voting to classify a new data point.

2. PROJECT OBJECTIVE

---

The main objective of this project is to understand and implement the internal
working of the K-Nearest Neighbors classification algorithm.

The program determines whether a new data point belongs to the Red or Blue
class based on the classes of its nearest neighboring points.

3. CASE STUDY

---

The dataset contains two-dimensional points represented using X and Y
coordinates.

Each existing point belongs to one of two classes:

* Red
* Blue

The program receives a new point:

X = 3
Y = 3

The KNN algorithm calculates the distance between this new point and every
existing point.

After calculating the distances, the points are sorted according to their
distance from the new point.

The K nearest points are selected and their class labels are counted.

The class receiving the highest number of votes becomes the final prediction.

4. DATASET

---

The dataset is manually created inside the Python program.

Data points:

Point A:
X = 1
Y = 2
Label = Red

Point B:
X = 2
Y = 3
Label = Red

Point C:
X = 3
Y = 1
Label = Blue

Point D:
X = 5
Y = 6
Label = Blue

Point E:
X = 6
Y = 6
Label = Blue

Point F:
X = 3
Y = 4
Label = Red

Point G:
X = 3
Y = 2
Label = Red

5. NEW DATA POINT

---

The point that needs to be classified is:

X = 3
Y = 3

The algorithm determines whether this point belongs to the Red or Blue class.

6. ALGORITHM

---

The implementation follows these steps:

Step 1:
Create a dataset containing X coordinate, Y coordinate and class label.

Step 2:
Define the new point that needs to be classified.

Step 3:
Calculate the Euclidean distance between the new point and every existing
data point.

Step 4:
Store the calculated distance with each data point.

Step 5:
Sort all data points according to their distance.

Step 6:
Select the K nearest neighbors.

Step 7:
Count the votes for each class.

Step 8:
Select the class having the highest number of votes.

Step 9:
Display the final prediction.

7. EUCLIDEAN DISTANCE

---

The Euclidean distance formula used in this project is:

Distance = sqrt((X1 - X2)^2 + (Y1 - Y2)^2)

The following user-defined function implements the formula:

MarvellousEucDistance(P1, P2)

This function calculates the distance between two points and returns the
calculated distance.

8. KNN IMPLEMENTATION

---

The main KNN logic is implemented in:

MarvellousKNNClassifier(K=3)

The function performs:

* Distance calculation
* Distance sorting
* Selection of nearest neighbors
* Voting
* Final classification

9. K VALUE

---

The program is executed with:

MarvellousKNNClassifier(5)

Therefore:

K = 5

The five nearest neighbors are considered for the final classification.

10. VOTING MECHANISM

---

After selecting the K nearest neighbors, the program counts the number of
votes received by each class.

Example:

Red   = Number of Red neighbors
Blue  = Number of Blue neighbors

The class with the highest number of votes is selected as the final prediction.

11. TECHNOLOGIES USED

---

Programming Language:

Python 3.10 or higher

Development Environment:

Visual Studio Code

Python Module Used:

math

12. LIBRARIES

---

This project intentionally uses only the Python standard library.

The math module is used for calculating the square root required by the
Euclidean distance formula.

No machine learning library is used for implementing KNN.

In particular, the project does not use:

* sklearn.neighbors.KNeighborsClassifier
* KNeighborsClassifier
* Any built-in KNN implementation

13. PROJECT STRUCTURE

---

KNN-Classifier-From-Scratch/
|
|-- knn_classifier.py
|-- README.txt
|-- requirements.txt

14. INSTALLATION

---

Requirement:

Python 3.10 or higher

Check the installed Python version:

python --version

Create a virtual environment:

python -m venv venv

Activate the virtual environment on Windows:

venv\Scripts\activate

15. DEPENDENCIES

---

This project does not require any third-party Python packages.

The only imported module is:

math

The math module is included with Python and does not need to be installed
separately.

16. EXECUTION

---

Run the program using:

python knn_classifier.py

The program displays:

* Original dataset
* Distance of every point from the new point
* Sorted data according to distance
* K nearest neighbors
* Voting results
* Final prediction

17. KEY CONCEPTS IMPLEMENTED

---

This project demonstrates practical implementation of:

* K-Nearest Neighbors
* Euclidean Distance
* Distance-based classification
* Sorting using a custom key
* Lambda functions
* Dictionary operations
* Majority voting
* User-defined functions
* Classification logic
* Python data structures

18. LEARNING OUTCOMES

---

Through this project, the following concepts are demonstrated:

* Understanding the working of KNN internally
* Implementing an ML algorithm without Scikit-learn
* Calculating Euclidean distance
* Finding nearest data points
* Implementing majority voting
* Understanding the importance of the K value
* Using Python dictionaries and lists for classification
* Building a simple classification system from scratch

19. FUTURE ENHANCEMENTS

---

Possible improvements include:

* Accept X and Y coordinates from the user.
* Allow the user to enter the value of K.
* Support more than two classes.
* Load data from a CSV file.
* Add graphical visualization of data points.
* Implement tie-breaking logic.
* Add distance-weighted voting.
* Compare the custom implementation with Scikit-learn KNN.
* Extend the implementation to support multiple features.

20. AUTHOR

---

Author:

Pratiksha Mahale

Project Type:

Machine Learning Algorithm Implementation

Algorithm:

K-Nearest Neighbors (KNN)

Implementation:

From Scratch using Python
