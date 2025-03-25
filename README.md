# Decision-Tree
My Self Learning For Decision Trees

Decision Trees Theory:
- Use data to decide how to break data into groups (i.e. fitting/training the model)
- This data is called training data
- The model can then be used to predict new outcomes with new data

Steps to Fitting the Model:
- Inspect variables in the data to determine what are the dependent and independent variables (can use columns property)
- Create subset x of independent variables and subset y of dependent variable
- fit to model of choice (in this case Decision Tree)
- use predict to view outcome
- validate the model to determine quality (can use vfarious metrics such as Mean Absolute Error(MAE))

When creating training data:
- best not to use same data to build and evaluate model
- model will be overfitted to the sample and will appear accurate but perform poorly in practice
- split data into 2 separate groups: training data and validation data (i.e. with train test split)

Method to Improve the Model:
- Overfitting and underfitting may occur for decision trees
    - Overfitting occurs with too many leaves as each prediction only depends on few data points
    - Underfitting occurs with too few leaves as each prediction has too many data points which results in the model failing to capture important distinctions and patterns
- Potential method to improve the model is specifying the number of max leaf nodes by looping through different values and comparing metrics

Random Forest Theory:
- Creates many decision trees and averages the predictions of each component tree

To Improve the Model:
- Specify number of n_estimators by looping through different values and comparing metrics

Dealing with Missing Data:
1) Drop Columns with Missing Values
    - Easiest option
    - Loses access to a lot of potentially useful information
2) Simple Imputation