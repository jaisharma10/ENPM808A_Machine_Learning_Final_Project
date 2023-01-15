# ENPM 808A --> Machine Learning Final Project

**Goal -->** to build regression models that can learn to predict translational valocity (v) amd angular velocity (w)
             based on lidar data, robot pose, final goal and local goals.

## Files

The folder jaisharma contains all the files relevant to the final project submission.

- report.pdf
- presentation.pptx
- code
  - data_cleaning.ipynb              <!-- goes over data cleaning and feature engineering steps -->
  - tune_deTree.ipynb                <!-- decision tree model -->
  - tune_nn.ipynb                    <!-- neural network model -->
  - tune_randF.ipynb                 <!-- random forest model -->
  - tune_sgd.ipynb                   <!-- linear regression with sgd model -->
  - tune_xgboost.ipynb               <!-- xg boost model -->
- figures

## Execution

All files within the folder 'Code' are ipynb files. They use relative paths to access the csv files. To run them, ensure 
that the folder 'Data' is within the Code folder. Or you could use abso;ute paths to access files from within your desktop.

Run each cell of code. Importing Training data can take up to 30 seconds. Training Model can take up to 2 minutes.

You can evaluate the performance of the model on two different test sets. In the Import Test Data cell, initialize the 
variable df_test with the test set of your choice.

## Support

For any questions, email me at jaisharm@umd.edu