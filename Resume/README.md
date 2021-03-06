## Math for ML
### Central Machine Learning Problems
- 3 major components in ML: 
  - data
  - models
  - learning
- The data is represented in tabular format by computer, that should be converted into numbers
- important to use domain knowledge when constructing the representation
- Even numerical data that could potentially be
directly read into a machine learning algorithm should be carefully 
considered for units, scaling, and constraints

_page 259_ 
- D-dimensional vector
  - N : number of examples in a dataset
  - n : index of examples (nth of N examples)
  - D : feature of interest about the example
  - d : 

3 Distinct algorithmic phases:
1. prediction/inference : the parameters and model choice is already
fixed and the predictor is applied to new vectors representing new input
data points
2. training/parameter estimation : adjust our predictive model based on 
training data.
3. hyperparameter tuning/model selection

LR: 264 (empirical risk minimization)
