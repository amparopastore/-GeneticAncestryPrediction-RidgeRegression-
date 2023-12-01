# CAP5625 - Programming Assignment 4 README

## Overview
This README provides instructions on how to run the provided program for Programming Assignment 3, focusing on implementing a penalized (regularized) logistic (multinomial) regression fit using ridge regression. The model parameters will be obtained by batch gradient descent. The goal is to predict an individual’s ancestry from genetic data projected along 𝑝=10 top principal components. Ridge regression will allow parameter shrinkage (tuning parameter 𝜆≥0) to mitigate overfitting. The tuning parameter 𝜆 will be chosen using five-fold cross-validation, and the best-fit model parameters will be inferred on the training dataset conditional on an optimal tuning parameter. This trained model will be used to predict ancestry on new test data points.

## Prerequisites
Before running the program, ensure you have the following prerequisites:

1. MATLAB installed on your computer.
2. The provided training dataset file named "TrainingData_N183_p10.csv" in the same directory as the MATLAB script.
3. The provided test dataset file named "TestData_N111_p10.csv" in the same directory as the MATLAB script.

## Running the Program
Follow these steps to run the program:

1. Open MATLAB on your computer.
2. Navigate to the directory containing the MATLAB script and the dataset files.
3. Open the MATLAB script (the file containing your program).
4. Run the script by clicking the "Run" button in the MATLAB Editor or by entering `run script_name.m` in the MATLAB command window, where `script_name.m` is the name of your script.

   For example: `run source_code.m`

The program will execute, performing ridge regression, batch gradient descent, and making predictions on the test data.

## Training Data
Training data for these observations are given in the attached "TrainingData_N183_p10.csv" comma-separated file, with individuals labeled on each row and input features (PC1, PC2, …, PC10) and ancestry label given on the columns.

## Test Data
Test data are given in the attached "TestData_N111_p10.csv" comma-separated file, with individuals labeled on each row and input features (PC1, PC2, …, PC10), and ancestry label given on the columns. There are five individuals with Unknown ancestry, 54 individuals with Mexican ancestry, and 52 individuals with African American ancestry. Each of the five Unknown individuals belongs to one of the five ancestries represented in the training set.

## Additional Notes
1. Ensure that the dataset files are correctly formatted and contain the required data columns for the program to execute successfully.
2. Make sure to have adequate computing resources, especially if you increase the number of iterations or use a large dataset, as training may take longer on slower hardware.
3. This README assumes a basic understanding of MATLAB. If you encounter any issues or have questions, refer to the MATLAB documentation.

Happy coding! 🚀
