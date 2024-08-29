# Medical Insurance Cost Prediction

This project predicts the medical insurance costs based on various features such as age, gender, BMI, number of children, smoking status, and region. The model is built using Linear Regression.

# Table of Contents

1.Dataset

2.Dependencies

3.Project Structure

4.Exploratory Data Analysis (EDA)

5.Data Preprocessing

6.Model Training

7.Evaluation

8.Usage Table of Contents

9.Dataset

10.Dependencies

11.Project Structure

12.Exploratory Data Analysis (EDA)

13.Data Preprocessing

14.Model Training

15.Evaluation

16.Usage

# Dataset

The dataset used in this project is a CSV file containing the following columns:

age: The age of the individual.

sex: Gender of the individual (male or female).

bmi: Body Mass Index, a measure of body fat based on height and weight.

children: Number of children/dependents covered by the insurance.

smoker: Smoking status of the individual (yes or no).

region: The individual's residential area in the US (southeast, southwest, northeast, northwest).

expenses: The medical insurance cost billed by the insurance company.

# Dependencies

To run the project, you need the following libraries:

Python 3.x

NumPy

Pandas

Matplotlib

Seaborn

scikit-learn

You can install the required libraries using the following command:

pip install numpy pandas matplotlib seaborn scikit-learn

# Project Structure

insurance.csv: The dataset file containing the medical insurance data.

insurance_cost_prediction.py: The main Python script for data exploration, preprocessing, model training, and evaluation.

# Exploratory Data Analysis (EDA)

Age Distribution: A histogram to visualize the distribution of ages in the dataset.

Sex Distribution: A count plot to show the distribution of gender.

BMI Distribution: A histogram to visualize the BMI distribution.

Children Distribution: A count plot to show the distribution of the number of children.

Smoker Distribution: A count plot to show the distribution of smokers and non-smokers.

Region Distribution: A count plot to show the distribution of regions.

Expenses Distribution: A histogram to visualize the distribution of medical insurance costs.

# Data Preprocessing

Encoding Categorical Variables: The sex, smoker, and region columns are encoded to numerical values for model training.

Feature and Target Separation: The dataset is split into features (X) and target (y).

Train-Test Split: The data is split into training and testing sets with an 80-20 ratio.

# Model Training

Linear Regression: The Linear Regression model is trained on the training dataset.

Prediction on Training Data: The model's performance is evaluated using R-squared value on the training data.

# Evaluation

The model's performance is evaluated using the R-squared value on both the training and test data. 
The R-squared value represents the proportion of the variance for the dependent variable that's explained by the independent variables.

Example output:

R squared value on training data: 0.7515

R squared value on test data: 0.7444

# Usage

To predict the insurance cost for a new individual, provide the input data as a tuple:

input_data = (age, sex, bmi, children, smoker, region)

Example input:

input_data = (31, 1, 25.74, 0, 1, 0)

Run the script, and the model will output the predicted insurance cost:

Example output:
The insurance cost is USD  3760.08
