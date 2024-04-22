# deep-learning-challenge
Module 21 Assignment


Report:
Testing (starter code) Notebook

1. Introduction:
In this report, we analysed and tested the optimisation process of several neural network models for predicting the 'IS_SUCCESSFUL' column in a dataset. The goal was to achieve a model accuracy of 75% or above. The dataset consists of various features, with 'IS_SUCCESSFUL' being the target variable. Two columns, 'EIN' and 'NAME', were dropped as they were neither targets nor features.

2. Model Experiments:

Original Model in AlphabetSoupCharity.ipynb:
Architecture: Two hidden layers with 15 nodes in layer 1 and 10 nodes in layer 2. Activations used - tanh layer 1 and relu layer 2 and output layer.
Result: Achieved accuracies of 72.46% (20 epochs) and 72.71% with (50 epochs) 30 more epochs used on model 1.

Model 1 in AlphabetSoupCharity_Optimisation.ipynb:
Architecture: Implimented and extra two hidden layers with 256 nodes in layer 1, 128 nodes in layer 2, 64 nodes in layer 3, and 32 nodes in layer 4. Activations used - relu for layer 1, 2, 3 and 4 and sigmoid for output layer. I tested sigmoid in place of relu and tanh in place of relu. Both gave lesser results.
Activation Functions: Replaced tanh with relu in hidden layers and used sigmoid for the output layer.
Result: Achieved an accuracy of 72.34%.

Model 2 in AlphabetSoupCharity_Optimisation.ipynb:
Architecture: Two hidden layers with 12 nodes in layer 1 and 6 nodes in layer 2. Activations used - tanh layer 1 and relu layer 2 and relu output layer.
Result: Achieved accuracies of 71.17%.

Model 3 in AlphabetSoupCharity_Optimisation.ipynb:
Architecture: Four hidden layers with 64 nodes in layer 1 and 32 nodes in layer 2, 16 nodes in layer 3 and 8 nodes in layer 4. Activations used - relu layer 1, 2, 3 and 4 and sigmoid  output layer. Epochs 20
Result: Achieved an accuracy of 72.34%.


AlphabetSoupCharity_Optimisation.ipynb

1. Column Removal:
Experimented with removing columns from the dataset to improve accuracy. I removed 3 columns 'STATUS', 'ORGANIZATION', 'USE_CASE' - this did not increase the results.

2. Increased Hidden Nodes:
Increased the number of hidden nodes in each layer: 256 in layer 1, 128 in layer 2, 64 in layer 3, and 32 in layer 4. This did not increase the results as expected. Results were 72.39%

3. Early Stopping:
Implemented early stopping to prevent overfitting.

Set a learning rate of 0.0001 and applied dropout of 0.5 to improve model performance.
4. Activation Functions:

Utilised relu activation for hidden layers and sigmoid for the output layer for better accuracy.

5. Conclusion:
Despite various optimisation attempts, including adjusting model architecture, hyperparameters, and preprocessing steps, the target accuracy of 75% was not achieved. The best-performing model achieved an accuracy of 72.34%. Further experimentation and fine-tuning may be necessary to improve the models performance.


 
