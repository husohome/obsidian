
# Hyperparameter Tuning

#dissertation
           
## Introduction version
The effectiveness of a model is not only decided by its parameters (e.g. weights/slopes and biases/intercepts), but also its configuration – called “hyperparameters” (e.g. how many layers; how many nodes each layer; what activation functions). Parameters are placeholders for quantities that could be estimated by the model using data; hyperparameters are placeholders for parameters. This section is about hyperparameters.

The model’s performance is naturally bounded by the quality of the parameter estimates, but hyperparameter could matter even more. For example, imagine an extreme case where the researcher sets up only one node and only one layer to subsume data that have 1000 input variables. Naturally the information will be reduced too much to cannot produce good prediction results. Thus, finding a good set of hyperparameters, a practice called “hyperparameter tuning”, is paramount for the model.

Of the hyperparameters for neural networks, the number of hidden layers and how many nodes for each layer, are the two most consequential, for the performance of the model. Thus, sometimes it suffices to manually do a series of experiments altering the values of these two and see which set up is optimal. However, as the neural networks become more complex, some advanced strategies might be worth employing. The following paragraph provides a quick summary.

**Grid Search.**  Grid search involves searching through a set of a predefined values of hyperparameters of concern. For example, the researcher may search through all of the combinations of 1 to 12 as the number of layers and 64 to 256 nodes for each layer.

**Random Search.** As each computation can be time-consuming, and there may be too many combinations (about 15000) to grid search for, an alternative strategy is use random search, which randomly picks some of the combinations and sees which ones give the best performance.

**Genetic Algorithm.** As random search may sound “unscientific” and too luck-dependent, some strategies, like genetic algorithms were developed. Genetic algorithms first draw a number of models, say 100, with random initial hyperparameters. Then, after the 100 models are fitted, the best performing subset, say the models with top 20 accuracy, are allowed to “reproduce”, which produces “children” that inherit some of the hyperparameters from each of their parent models, and randomly “mutate” a few hyperparameters for their idiosyncrasies. The same culling and reproduction cycle is repeated a few times, say 20, and the researcher reaps the fittest of them all “after generations of evolution”.

