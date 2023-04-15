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

## Limitation 

Naive Bayes assumes that features are independent, which is often not true in real-world situations. This can lead to poor performance when features are correlated.

The algorithm assumes data is normally distributed. If the data is not Gaussian, the classifier might not perform well.

The classifier works well with continuous features, but it might not be the best choice for categorical features with many categories.

## Bayes' theorem is a rule in probability theory that helps us find the probability of an event occurring based on new information. It's a way of updating our beliefs when we have new evidence. The formula for Bayes' theorem is:

P(A|B) = (P(B|A) * P(A)) / P(B)

Here's what each term means:

P(A|B): The probability of event A happening given that event B has occurred. This is called the "posterior probability."
P(B|A): The probability of event B happening given that event A has occurred. This is called the "likelihood."
P(A): The probability of event A happening without any information about event B. This is called the "prior probability."
P(B): The probability of event B happening without any information about event A.
Let's go through a simple example:

Imagine you have a bag with 100 marbles. There are 30 red marbles and 70 blue marbles. You know that 20 of the red marbles have a special symbol on them, and 10 of the blue marbles have the same symbol.

Now, if you pick a marble with the symbol, what is the probability that it's red?

We can use Bayes' theorem to find the answer. In this case, event A is picking a red marble, and event B is picking a marble with the symbol.

P(A) = 30/100 (There are 30 red marbles in total)
P(B|A) = 20/30 (20 red marbles have the symbol)
P(B) = (20 red marbles with the symbol + 10 blue marbles with the symbol) / 100 = 30/100
Now, we can use the formula:

P(A|B) = (P(B|A) * P(A)) / P(B) = (20/30 * 30/100) / (30/100) = 20/30

So, the probability of picking a red marble given that it has the symbol is 20/30 or approximately 0.67 (67%).
