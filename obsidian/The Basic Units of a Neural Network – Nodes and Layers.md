# The Basic Units of a Neural Network – Nodes and Layers[[SH1]](#_msocom_1) 

#dissertation 


The building blocks of a neural network are “nodes” (e.g., Chollet, 2017; Anthony, & Bartlett, 2009), which are linear regression results transformed by a non-linear activation function (Warner, & Misra, 1996). That is, a node is a statistically constructed variable whose values are only possible after the weights and intercept are estimated by the model. The left panel of Figure 3.2 shows a simplified example of a node (a circle) receiving three input variables (predicted by three observed variables, in squares). Node 1 is the weighted sum of [X1, X2, X3] by [w1, w2, w3] plus an intercept term, _b_, called “bias” in machine learning parlance.

 The right panel of Figure 3.2 shows two other nodes that are fitted using the same input variables, [X1, X2, X3] as in Node 1, but the weights might be different, say [w4, w5, w6] and [w7, w8, w9].

 In addition to the “weighted sums plus intercept”, called an “affine transformation” in linear algebra”, each node goes through a non-linear transformation using what is called the activation function of choice, addressed slightly later. For now, the non-linear activation function is denoted as _f._ Node 1 is therefore the affine-transformed and [X1, X2, X3] by [W1, W2, W3] plus intercept _b_, fed to _f_, which we denote as _f_(WTX + b) here. Node 2 and Node 3 can also be expressed similarly, with different _W_ and _b_ but the same _X_.

 Figure 3.2.

_Example Nodes in Neural Network_  

**_Note._** Left panel: a single Node that receives input directly from observed data. Right panel: a (dense) layer of nodes that receives input from the input data; the bias term is not shown to keep the figure clean.

Nodes may also be receiving input from other nodes as shown in Figure 3.3 where Nodes 4 and 5 receive input from Node 1, 2 and 3. That is, they weigh [Node 1, Node 2, Node 3] by some differently estimated weights, add an intercept and feed the affine-transformed results to a non-linear function. The last layer, “output layer”, is [Node 4, Node 5] weighted differently plus a differently estimated intercept and fed to a non-linear transformation.

Figure 3.3 _The Basic Structure of a Neural Network_  

_Note._ This figure is just for illustration purposes and does not reflect the actual model used in the current study.

The output layer works the same as the hidden layers, except the values of them are interpreted as the model predictions of the outcome values. The nodes in the output layer (in Figure 3.3, Node 7, 8 and 9) would each represent one outcome category. The fact that there are three nodes in the neural network specified in Figure 3.3 means there are three categories. For the convenience of understanding, let’s assume Node 6, 7, and 8 correspond to the categories 1, 2, and 3 respectively. Importantly, since the output layer, third layer counting from (exclusive of) the raw data (i.e., input layer), the nodes would have gone through three pairs of affine-and-non-linear transformations.

 To deepen understanding, let’s link the neural network back to regression models. It should hopefully be clear by now that a neural network is regressions which take input from previous non-linear regressions. An ordinary linear regression can be thought of as one node that directly takes input from the raw data with no activation function applied. A logistic regression is one node that directly takes input from the raw data with the sigmoid activation function. Conversely, a neural network is a series of nonlinear regressions that lead to the final layers of outcomes.

---

 [[SH1]](#_msoanchor_1)Original version was

The basis of neural networks is the old and familiar linear regression, which can be expressed as this:  , where _y_ is a vector of all the predicted variables, _b_ is the “bias” term, the machine learning term for an intercept, and _W_ is a vector containing all “weights” for the all predictors, which are the machine learning term for regression coefficients. _X_ is a vector containing the value of all the predictors_. WTX_ is the dot product of _W_ and _X_, which is the linear algebra notation (consistent with that used in a widely used Linear Algebra textbook by Mal'tsev, 1963) for the weighted sum of predictors and coefficients, which is .

When the outcome is categorical, its linear relationship with the predictors is formulated via a nonlinear link function. The following is a typical logistic regression, where the predicted outcome variable y is dichotomous (1 and 0). The natural log of odds (i.e., logit) is expressed as a linear combination of the predictors given as,

,

which can be non-linearly transformed to the probability of outcome being 1 (vs. 0), given as

This non-linear transformation is important for the understanding of neural networks. In fact, in neural network terms, the non-linear link function is called an “activation function”, of which a commonly used type is the sigmoid, which is exactly the same as the logit link function. The following notation, adapted from what is commonly used in the neural network literature, highlights this view:

 Where the  is the activation function,  is the vector of model-predicted _y_s, which is .

In neural networks, the activation function could be other options of the user’s choice, and the above expression illustrates the sigmoid function, but no matter which one, it will be denoted as  in the following introduction.