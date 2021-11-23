       

# Neural Networks are Regression-Like

#dissertation 

Machine learning is about making computers run statistics and make decisions and neural networks, like regression models, are a particular way to run statistics. Indeed, a basic neural network, called a feedforward neural network, is regression-like (Warner & Misra, 1996). It can be thought of as a series of regressions, where the following regression is regressed upon the result of its immediately preceding regression. The first in the series, which has no predecessors, is regressed on the data, whereas the last, which has no followers, needs to output, usually, the probabilities of outcome categories. The regressions are always non-linear, where each regression is a linear regression fed to a non-linear transformation.