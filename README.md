## Linear Regression for Salary Prediction
This project implements a simple linear regression model to predict salaries based on years of work experience.

### Description
The model uses gradient descent to minimize the loss function (Mean Squared Error) and find the best-fit line for the given data. The algorithm iteratively updates the slope and intercept of the line to minimize the average squared difference between the predicted and actual salaries.

### Math Flow
Initialize model parameters: Set the initial slope (m) and intercept (b) to zero.
Implement gradient descent:
Calculate the gradients of the loss function with respect to the slope and intercept.
The slope gradient is: ∂L/∂m = −2n∑i=1nxi(yi−y^i)∂m∂L​ =−n2​ ∑i=1n xi (yi −y^i )
The intercept gradient is: ∂L∂b=−2n∑i=1n(yi−y^i)∂b∂L​ =−n2​ ∑i=1n​ (yi −y^​i )

Update the slope and intercept using the calculated gradients and a learning rate (α).
Repeat the gradient calculation and update steps for a specified number of epochs.
Predict salaries: Use the final slope and intercept to predict salaries for new data points.

### Code Flow
Load the dataset: Read the "Salary_Data.csv" file containing years of experience and corresponding salaries.
Visualize the data: Create a scatter plot of years of experience vs. salaries to understand the relationship.
Define the gradient descent function:
- Calculate the slope and intercept gradients based on the current parameters and the dataset.
- Update the slope and intercept using the gradients and the learning rate.
Train the model: 
- Initialize the slope and intercept to zero.
- Run the gradient descent function for a specified number of epochs.
- Print the slope and intercept at regular intervals to monitor the training progress.
- Plot the best-fit line: After training, plot the original data points and the best-fit line using the final slope and intercept.

### Usage
Ensure you have the required dependencies installed (pandas, matplotlib).
Run the main script to train the model and visualize the results.
