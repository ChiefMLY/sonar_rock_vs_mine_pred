# Machine Learning Project - Rock vs Mine Classification (sonar)

This project aims to build a machine learning model to classify sonar data as either a rock or a mine. The dataset used in this project contains various features representing sonar signals and corresponding labels indicating the class of the signal.

## Dataset
The dataset used in this project is stored in the file "sonar data.csv". It contains 208 rows and 61 columns. Each row represents a sonar signal, and the last column (column 60) contains the labels ('R' for rock and 'M' for mine). The remaining columns represent the features extracted from the sonar signals.

## Explanatory Data Analysis
Before building the machine learning model, some exploratory data analysis was performed on the dataset. Here are some key observations:

- The dataset has 208 rows and 61 columns.
- There are no missing values in the dataset.
- The dataset contains 60 numeric feature columns and 1 categorical label column.
- The statistical summary of the dataset shows the count, mean, standard deviation, minimum, 25th percentile, median, 75th percentile, and maximum values for each feature column.
- The dataset is imbalanced, with 111 instances labeled as 'M' (mine) and 97 instances labeled as 'R' (rock).

## Model Training - Logistic Regression
The machine learning model used for this classification task is Logistic Regression. The following steps were performed:

1. The dataset was split into the data (X) and labels (y).
2. The data and labels were further split into training and test sets using a test size of 10% and stratified sampling to maintain the class distribution.
3. Logistic Regression model was trained using the training data.
4. The model's accuracy was evaluated on both the training and test data.

The accuracy of the Logistic Regression model was found to be 83.42% on the training data and 76.19% on the test data.

## Predictive System
To demonstrate the model's predictive capability, a known data point (labeled as a rock) was inputted into the model to see if it correctly predicts the label. The model successfully predicted the label for the given input.

## Usage
To reproduce the results and use this project:

1. Download the "sonar data.csv" file and place it in the same directory as the project code.
2. Run the code in a Python environment with the required dependencies installed.
3. The code will load the dataset, perform data analysis, train a Logistic Regression model, evaluate its accuracy, and provide a predictive system example.

Please note that the code assumes the availability of the required Python libraries, such as pandas, scikit-learn (with LogisticRegression, train_test_split, and accuracy_score), and numpy.

Feel free to modify the code or dataset to suit your specific needs.

## License
This project is released under the [MIT License](https://opensource.org/licenses/MIT).
