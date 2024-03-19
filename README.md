# Startup-Sucess-Prediction

## Objective:
The objective of this notebook is to predict whether a startup, currently operating, will turn into a success or failure. Success is defined as a company achieving a large sum of money through M&A (Merger and Acquisition) or an IPO (Initial Public Offering), while failure refers to a company being shut down.

## About the Data:
The dataset contains industry trends, investment insights, and individual company information. It comprises 48 columns/features, including quantitative and categorical variables such as funding rounds, relationships, industry type, and state. The target variable is the status of the startup (acquired or closed).

## Dataset Description:
Startups play a crucial role in economic growth by bringing new ideas, spurring innovation, and creating employment opportunities. This dataset aims to analyze startup data to predict their success, assisting investors in identifying companies with potential for rapid growth.

## Acknowledgements:
- Dataset provided by Ramkishan Panthena, a Machine Learning Engineer at GMO.
- Used in data sprint #5 at DPhi.

## Inspiration:
Predicting startup success enables investors to identify high-growth potential companies, giving them a competitive edge in the market.

## Evaluation:
The evaluation metric for this competition is Categorization Accuracy. Submissions should be in CSV format with two columns: ID and status, where status indicates whether the startup is acquired or closed.

## Notebook Structure:
1. **Importing Modules:** Necessary Python libraries such as pandas and numpy are imported for data manipulation.
2. **File Path and Reading:** The dataset is loaded from the specified file path using pandas' `read_excel` function.
3. **Checking for Null Values:** Null values in the dataset are identified and summarized.
4. **Data Preprocessing:** 
    - Columns with a high number of null values are dropped.
    - Missing values in certain columns are filled with appropriate values.
    - Data normalization is performed to bring numerical features to a similar scale.
    - Categorical variables are one-hot encoded for modeling.
5. **Train-Test Split:** The dataset is split into training and testing sets for model evaluation.
6. **Model Building and Evaluation:**
    - Logistic Regression and Support Vector Classification (SVC) models are implemented and evaluated using cross-validation.
    - The accuracy of each model is assessed on both training and testing sets.
7. **Predictions on Test Data:** 
    - Test data is loaded and preprocessed similarly to the training data.
    - The trained model is used to make predictions on the test data.
8. **Final Submission Preparation:** 
    - Predicted results are mapped to appropriate categories (acquired or closed).
    - Final submission file containing ID and status columns is prepared and saved as a CSV file.

## Note:
- The notebook provides a comprehensive analysis of startup success prediction, from data exploration to model evaluation.


