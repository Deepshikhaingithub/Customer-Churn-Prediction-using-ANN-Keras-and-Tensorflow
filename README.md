# Customer-Churn-Prediction-using-ANN-Keras-and-Tensorflow

Project Overview:
This project aims to develop a predictive model that can effectively identify customers who are likely to exit a multinational bank operating in France, Spain, and Germany. Customer churn, the act of customers leaving the bank, is a critical concern for financial institutions. Understanding and predicting churn can help the bank take proactive measures to retain valuable customers, thereby reducing revenue loss and maintaining a competitive edge in the market.

Data Description:

The dataset contains the following columns:

RowNumber: A unique identifier for each row.

CustomerId: A unique identifier for each customer.

Surname: The surname of the customer.

CreditScore: The credit score of the customer.

Geography: The country in which the customer resides (France, Spain, or Germany).

Gender: The gender of the customer (Male or Female).

Age: The age of the customer.

Tenure: The number of years the customer has been with the bank.

Balance: The account balance of the customer.

NumOfProducts: The number of bank products the customer uses.

HasCrCard: Whether the customer has a credit card (1 for yes, 0 for no).

IsActiveMember: Whether the customer is an active member (1 for yes, 0 for no).

EstimatedSalary: The estimated salary of the customer.

Exited: The target variable, indicating whether the customer has exited the bank (1 for yes, 0 for no).

Steps taken for implementing the project:

1. Data Cleaning:

-- Preprocessed the dataset to handle missing values, if any.

2. Balanced the Dataset using SMOTE:

--Addressed class imbalance in the dataset using Synthetic Minority Over-sampling Technique (SMOTE) to create synthetic samples of the minority class.

3. Feature Selection:

-- Selected only the relevant columns/features required for the customer churn prediction task, including columns like 'CreditScore,' 'Geography,' 'Gender,' 'Age,' 'Tenure,' 'Balance,' 'NumOfProducts,' 'HasCrCard,' 'IsActiveMember,' and 'EstimatedSalary.'

4. Categorical Variable Encoding:

-- Converted categorical variables ('Geography' and 'Gender') into numerical format using pd.factorize.

5. Standard Scaling:

-- Applied standard scaling to the numerical features to ensure that all features have the same scale before feeding them into the Artificial Neural Network (ANN) model.

6. ANN Model Development:

-- Created an Artificial Neural Network (ANN) model using Keras.

-- Utilized the Sequential API to build the neural network.

--Defined layers using Dense layers to specify the architecture of the model.

7. Weight Initialization:

-- Initialized the weights and biases in the neural network. Weight initialization can affect the training process and model performance.

8. Model Compilation:

-- Compiled the ANN model by specifying the loss function, optimizer, and evaluation metrics.
-- Commonly used loss functions for binary classification tasks include 'binary_crossentropy.'
-- Selected an optimizer (e.g., Adam) and metrics (e.g., accuracy) suitable for the task.

9.Model Training:

--Trained the ANN model on the preprocessed and balanced dataset using training data.

10. Model Evaluation:

-- Evaluated the model's performance using appropriate metrics, such as accuracy score to assess its effectiveness in predicting customer churn.

11. Predictions on New Data:

-- Deployed the trained model to make predictions on new, incoming data to identify potential customer churn cases.

****CONCLUSION****

In conclusion, this customer churn prediction project has yielded promising results with an accuracy score of 83%. The project involved meticulous data preprocessing, including data cleaning, feature selection, and encoding of categorical variables. We addressed class imbalance using SMOTE, ensuring a more robust model.

The Artificial Neural Network (ANN) model built using Keras demonstrated its effectiveness in identifying potential customer churn cases within the bank's clientele. This accuracy score of 83% suggests that our model can make reasonably accurate predictions.

This project not only developed a predictive models but also highlights the potential for proactive customer retention strategies within the banking industry. Further refinements and optimizations can enhance the model's predictive power and provide valuable insights to the bank for reducing churn and ensuring customer satisfaction.
