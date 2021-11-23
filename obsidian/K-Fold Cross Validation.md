                   

# K-Fold Cross Validation    
#dissertation

In fitting the neural network model, it is common to follow a K-fold cross validation procedure, illustrated in Figure 3.4, which shows a common case where K = 5, called a five-fold cross validation (Chollet, 2017; Géron, 2019). The data are separated into K + 1 equally sized parts, with one part called the “test” data, one part called the “validation” data and the remaining K -1 parts (in this case 4) called the “train(ing)” data. Figure 3.4 shows an illustrative case of a five-fold validation with 6000 rows in the data. This means the test data contain 1000 rows, validation data 1000 rows and train data, 4000. The real data in the current consists of 9443 rows; the 6000 in Figure 3.4 is just to facilitate understanding.

Figure 3.4

  
_An Illustration of Five-fold Validation of a Mock Data Set with 6000 Observations_

The five-fold cross validation fits the data five times (= K). Each time a different part of the data is used as the validation data. As in Figure 3.4, for example, the first time of training uses the first 1000 rows as the validation data, the second time uses the 1000th to the 2000th rows, and so on, when the last time the last 1000 rows are used as the validation data.

The train data is essentially the only available data used for actually fitting the neural network model. That is, the neural network is pretending not to see the validation data and the test data, and the weights and biases are obtained only on the basis of the different set of 4000 rows assigned train data each time, as in Figure 3.4. Each time, after the training with the 4000 rows of data, the model applies the weights and biases both to the validation data, which are also different each time, and to the test data, which are the same across all the K times of training. As such, each time, for each performance metric, two sets are obtained. One set reflects how well the model generalizes to the validation data, and the other, how well it does the test data. In the current study, which reports both F1-gain, and Precision-gain, there are four sets: F1-gain for validation data, F1-gain for test data, Precision-gain for validation data, and Precision-gain for test data – four “sets” of values because each major has their own values for the performance metrics.

The reason K-fold cross validation becomes a convention is that neural networks are known to fit data well, and the model may adapt to the data too well that it fails to generalize. K-fold cross validation provides a good way to see if the performance of the model is due to the haphazard split of the data. If the generalization performance metrics on validation and test data sets are similar across the five times, then there is not too much heterogeneity in the full data to worry about. Also, averaging the five times provides a more unbiased measure of the performance of the model.

The current study adopts a five-fold cross validation with the same steps as illustrated in Figure 3.4, except the data have 9443 rows, instead of 6000. That is, one part is 1574 rows, which is 1/6 of the entire respondents of 9443. All the results are the averages of the five times of training of the four sets of performance indexes. This will become clear in Results.