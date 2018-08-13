# Ame-House-Price

## Dependency
- sklearn
- matplotlib
- seaborn
- missingno
- pandas
- fancyimpute
- scipy
- xgboost
- lightgbm
- catboost

And also you need jupyter notebook to run the notebook.

## Result
You need to tune a little bit to get my final score RMSE: 0.11425

## Tips:
1. Different version of dataset works differently on same model. Make sure your dataset fits your model.
  - Tree based models work not so well on one-hot encoded features. But linear/SVM/Neural Network model is good at it.
  - Feature generation is important. Models cannot make cross feature implicitly by themselves easily, so you need to do it explicitly.

2. Training stacked model may easily suffer from overfitting. You need keep the OOF prediction from the first layer models and fit it to the second layer model as training set.

3. Don't trust your hand for tunning hyperparameters. Trust random search or grid search instead.

4. Use visualization to figure out your problem.
