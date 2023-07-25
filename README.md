Linear Regression in Python
This Python class implements a simple linear regression model using gradient descent for learning. The linear regression model aims to find a relationship between one or more features(independent variables) and a continuous target variable(dependent variable).

Class: LinearRegression
Methods:
__init__(self, learning_rate, iterations)

The constructor method of the class. It initializes the model with specified learning rate and number of iterations to perform gradient descent.

fit(self, X, Y)

This method trains the model using the input data X and target values Y. It initializes the weights and bias to zero, and then updates these parameters using gradient descent.

update_weights(self)

This is a helper method for the fit method. It computes the gradient of the loss with respect to the weights and bias, and then updates these parameters in the direction of the negative gradient. The size of the step taken in the negative gradient direction is determined by the learning rate.

predict(self, X)

Once the model is trained, this method makes predictions on new data X. It computes the dot product of X with the weights and adds the bias.

Attributes:
learning_rate

The learning rate for gradient descent.

iterations

The number of iterations for which to run gradient descent.

m, n

The dimensions of the input data X.

W

The weights of the linear regression model. After training, these weights represent the coefficients of the features in the target function.

b

The bias of the linear regression model. After training, this bias represents the intercept of the target function.

X, Y

The training data and target values that the model was trained on.

The code is written in Python and uses NumPy for operations on arrays. It is a simple, yet powerful, implementation of one of the foundational models in machine learning.
