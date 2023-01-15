# ENPM 808A --> Machine Learning Final Project

## Introduction

This is my final project submission for ENPM808A -  Introduction to Machine Learning course. The course was taken in the Fall of 2022 semester at the University of Maryland. 

We are provided with a novel dataset on which we need to perform regression. The data comes from multiple path planning MPC tests conducted with a car-like robot model. The data is stored in multiple CSV files and organized in columns as follows:

- Laser Range - 1:1080
- Final Goal (x,y,qk,qr) – 1081:1084
- Local Goal (x,y,qk,qr) – 1085:1088
- Pose (x,y,qk,qr) – 1089:1090
- Cmd_vel_v - 1091
- Cmd_vel_w - 1092

**Goal -->** to build regression models that can learn to predict translational valocity (𝑣), and angular velocity (𝑤) 
             based on lidar data, robot pose, final goal and local goals.

## Files

The folder 'code' contains all the files relevant to the final project submission.



## Execution

All files within the folder 'Code' are ipynb files. 

  - data_cleaning.ipynb       &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;       # goes over data cleaning and feature engineering steps 
  - tune_deTree.ipynb        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;        # decision tree model 
  - tune_nn.ipynb           &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;         # neural network model 
  - tune_randF.ipynb        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;         # random forest model 
  - tune_sgd.ipynb          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;         # linear regression with sgd model 
  - tune_xgboost.ipynb      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;         # xg boost model 

They use relative paths to access the csv files. To run them, ensure that the folder 'Data' is within the Code folder. Or you could use absolute paths to access files from within your desktop. Run each cell of code. Importing Training data can take up to 30 seconds. Training Model can take up to 2 minutes. You can evaluate the performance of the model on two different test sets. In the 'Import Test Data' cell, initialize the variable 'df_test' with the test set of your choice.

## Support

For any questions, email me at jaisharm@umd.edu
