# Churn Modeling Project
## Overview
This project focuses on building a churn prediction model using machine learning techniques. The workflow includes data preprocessing, feature engineering, model training, and deployment.

## Dataset

**Source:** Churn dataset containing customer information.
**Columns:**
- `RowNumber`: Unique row identifier.
- `CustomerId`: Unique customer identifier.
- `Surname`: Customer's surname.
- `CreditScore`: Customer's credit score.
- `Geography`: Customer's location (e.g., France, Spain).
- `Gender`: Customer's gender (Male/Female).
- `Age`: Customer's age.
- `Tenure`: Number of years the customer has been with the bank.
- `Balance`: Customer's account balance.
- `NumOfProducts`: Number of bank products the customer uses.
- `HasCrCard`: Whether the customer has a credit card (1 = Yes, 0 = No).
- `IsActiveMember`: Whether the customer is an active member (1 = Yes, 0 = No).
- `EstimatedSalary`: Customer's estimated salary.
- `Exited`: Whether the customer has left the bank (1 = Exited, 0 = Remained).


**Dataset Size:** 10,000 customers.
**Churn Analysis (Estimated):**
- Based on a sample of 7 customers:
  - Customers who exited (Exited = 1): 3
  - Customers who remained (Exited = 0): 4 (57.14%)


- Estimated remaining customers in the full dataset: ~57.14% of 10,000 = approximately 5,714 customers.
- Note: This is an estimation based on a small sample and may not reflect the actual churn rate in the full dataset.



## Workflow
**1. Dataset**

- **Source:** Input dataset for churn modeling (as described above).

**2. Classification**

**Preprocessing:**
- Convert categorical variables (e.g., Geography, Gender).
- Handle missing values.
- Numerical standardization (e.g., CreditScore, Balance, EstimatedSalary).

**3. Basic Feature Engineering (FE)**

- Process: Basic feature extraction and transformation.

**4. Model Architecture**

- **Input Layer (IP Layer):** Initial layer for input data.
- **Dropout:** Applied to prevent overfitting.
- **Optimizers:** Used to optimize the model.
- **Keras/TensorFlow:** Frameworks for building and training the model.

**5. Model Output**

- **Pickle:** Model saved in pickle format.
- **H5 File Format:** Alternative model storage format.

**6. Deployment**

- **Streamlit:** Web app for model deployment.
- **Streamlit Cloud:** Hosting the deployed model.

## Notes

- Ensure to avoid overfitting during training.
- The pipeline integrates various steps from data preprocessing to model deployment.

**Tools & Technologies**

- Python (Keras, TensorFlow)
- Streamlit
- Pickle- H5 file format

## Next Steps

- Test the deployed web app.
- Monitor model performance and retrain as needed.





