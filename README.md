# Non-Linear-Regression-to-Multivariable-non-Linear-Regression
- Preprocessing data (dealing with null, ...)
- EDA (Explore Data Analysis): Correlation between features and labels, Linear function or non-linear function, 2-degree or 3-degree,...
- Representation: Data transformation by using Label Encoding / One hot encoding, ...
- Modeling: training and evaluation
- Deployment
## Important Note:
- Degree Choice: if too simple, model would not flexible enough (underfit), if too complicate, model would overfit
- ![choiceofdegree](https://drive.google.com/uc?export=view&id=1RF7FuCVyqebv3is16rPLQ0S6AahrkOec)
- Good method for choice of the degree: k-fold cross-validation
  + Example: suppose we have 1000 samples: 800 training and 200 testing
    * focus on training set, testing set only be used to evaluate model.
    * The original dataset is divided into K equal-sized subsets or folds.
    * The model is trained and evaluated K times.
    * In each iteration, K-1 folds are used for training the model, and the remaining fold is used for testing/validation.
    * ![kfold](https://miro.medium.com/v2/resize:fit:1200/1*AAwIlHM8TpAVe4l2FihNUQ.png)
    * The performance metric (such as accuracy or mean squared error) is computed for each iteration.
    * The final performance measure is obtained by averaging the results from all K iterations.
    * Choose the degree which has the lowest out of sample error
   
