# Iris_classification_by_naive_bayes-GUI-


This project uses a Gaussian Naive Bayes classifier to predict the species of an iris plant based on its sepal length, sepal width, petal length, and petal width. The Iris dataset is used for training and testing the classifier. The code also includes a GUI built using ipywidgets, which allows users to input the sepal length, sepal width, petal length, and petal width of an iris plant and receive a prediction of its species.

## Requirements
- scikit-learn
- ipywidgets

## Usage
To use the GUI, run the code in a Jupyter notebook. Four float sliders will appear, representing the sepal length, sepal width, petal length, and petal width of an iris plant. The user can adjust the values of the sliders and press the submit button to receive a prediction of the plant's species.

## Code Summary
- The Iris dataset is loaded and split into training and test sets.
- A Gaussian Naive Bayes classifier is created and trained on the training data.
- A `predict_species` function is defined to accept the sepal length, sepal width, petal length, and petal width of an iris plant as inputs and return a prediction of its species.
- The GUI is created using ipywidgets, including four float sliders for the sepal length, sepal width, petal length, and petal width, a submit button, and an output label to display the prediction.
- The `on_submit_clicked` function is defined to handle the click event of the submit button and display the prediction in the output label.
