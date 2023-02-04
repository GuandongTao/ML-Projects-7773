Implemented a momentum-based trading strategy for SPY, following the J.P.Morgan research document "Example of Penalized Regression Approach in a Multi Asset Trend 
Following Strategy".

For predictor variables, choose lagged 1W, 2W, 1M and 2M returns of S&P and 3 other Indices (Any ticker in the directory beginning with the letter "X" is an index; 
so XLK is the technology sector index), yielding a total of 16 variables. To calibrate the model, we used a rolling window of 100 trading days (~); re-calibration 
is performed once every month. The model will be used to predict the next day's return for S&P. If the next day predicted return is positive, you go long the asset, 
otherwise you short it.

The following learning algorithms were evaluated: 
Ordinary Least Squares, Lasso, Ridge, ElasticNet, and kNN
