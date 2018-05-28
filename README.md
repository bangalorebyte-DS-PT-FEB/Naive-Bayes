# Naive-Bayes

To understand Naive Bayes approach to classification modelling, here are two datasets. One has only continous features, the other has both continous and discrete. Use a Gaussian NB (scikit-learn.org/stable/modules/generated/sklearn.naive_bayes.GaussianNB.html)  model to fit the Default dataset. For the Prima Indian data (https://www.kaggle.com/uciml/pima-indians-diabetes-database) however, I want you to try and compare two approaches. 

First, split the cotinous and discrete features in the model. Fit the target and discrete features only with a Multinomial NB model (http://scikit-learn.org/stable/modules/generated/sklearn.naive_bayes.MultinomialNB.html#sklearn.naive_bayes.MultinomialNB_ . Then fit the target and continous features with the Guassian NB. Now what you should have is two lists of probabilities for each validation dataset. Multiply the two lists with element wise to get a single list of proabilities. 

Compare the above approach to simply fitting both discrete and contious features with a Gaussian NB model. Read more about the different NB models at: http://scikit-learn.org/stable/modules/naive_bayes.html

So, you should compare the preceision and recall scores of the above approaches. 
