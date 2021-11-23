           

# Activation Functions

#dissertation 

As a commonly used activation function, the sigmoid function is the same as the nonlinear transformation from logits to probabilities in logistic regression. It transforms the linear combination of nodes in previous layers, _m_, into . The sigmoid activation function yields a value ranging from 0 to 1, which is ideal if the value needs to be interpreted as a probability. As such, the sigmoid function is used in the outcome layer in the multilabel neural network in the current study, where the values are the predicted probabilities that the majors are in the respondents’ top 3.

Another common activation function is hyperbolic tangent, _tanh_, which is , which forces the value to fall between -1 and 1. Finally, the Rectified Linear Unit, ReLU, which is _m_,  _m_ > 0, and 0  _m_  0, is commonly used in hidden layers for its computational efficiency and good performance (e.g., Ketkar, 2017; Chollet, 2017).

The activation function of the output layer is decided by the type of output the user needs. Most commonly, one might want a real-valued prediction, as in a linear regression model, or the probability of the “yes” category in a dichotomy, as in a logistic regression, or list of probabilities for some categories, as in multinomial logistic regression. In the case of CMPA shortening, we used Sigmoid, for dichotomous prediction for each of the 50 majors.