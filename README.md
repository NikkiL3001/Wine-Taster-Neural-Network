# Wine Taster Neural Network

Wine Taster Neural Network attempting to predict human wine taster quality scores based on physicochemical data. 

The two datasets are red and white *vinho verde* wine samples from Portugal. The datasets are available from the UCI machine learning repository, https://archive.ics.uci.edu/ml/datasets/wine+quality. The data was first published in *P. Cortez, A. Cerdeira, F. Almeida, T. Matos and J. Reis. Modeling wine preferences by data mining from physicochemical properties. In Decision Support Systems, Elsevier, 47(4):547-553, 2009*.

11 physicochemical attributes are used as inputs to the NN with the output a quality score between 0 (very bad) and 10 (excellent). 

In **regression_red_wine**, the prediction of the quality score is done as a regression problem using the red wine dataset. 

In **binary_classification_white_wine**, the white wine samples are classified into one of two categories corresponding to good (0-5) and better (6-10) wines.

Finally, in **classification_white_wine**, the white wine samples are classified into 11 classes corresponding to the quality scores (0-10). Here the problem of overfitting is studied by using varying size NNs. Overfitting is addressed with regularization techniques and comparisons between NNs are made.

<img src="https://github.com/NikkiL3001/Wine-Taster-Neural-Network/blob/master/Model_performance.png" width="561" height="367">
Adding L2 and dropout regularization to a large model suffering from overfitting improves the results significantly even compared to a small simple model.
