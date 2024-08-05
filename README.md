# Home Equity Lines of Credit (HELOC) Classification Project
## Introduction
The goal of this project is to develop a machine learning model to predict whether a customer will pay back their Home Equity Line of Credit (HELOC) within two years based on attributes in their loan application. The model will be trained using the Huggingface HELOC dataset provided by FICO.

## Business Application and Impact
### This project aims to enhance the efficiency and accuracy of the HELOC application process. Specifically, it will:

- Improve Application Response Time: By automating the classification process, faster decisions on applications can be made.
- Maximize 'Goods' and Minimize 'Bads': The model will aim to correctly identify credit-worthy applicants ('goods') and reject non-credit-worthy ones ('bads'), thereby improving overall revenue generation.

### Impacts:
- Optimized Business Processes: Automation of the classification process saves time and money, reduces employee workload, and allows staff to focus on more complex tasks.
- Reduced Human Bias: Historically, loan decisions were made at the discretion of Loan Officers, whose decisions were influenced by their experience and potential implicit biases. The model uses concrete data to make decisions, reducing the risk of misclassification due to human error or bias.
- Improved Decision Explanation: The model provides explainable results, enabling communication of reasons for denial to applicants. This transparency helps applicants understand and improve on the factors influencing their application outcomes, such as income, debt levels, credit scores, or credit history length.

## Literature Review
- [HELOC Risk Prediction - Siyuan Feng](https://siyuan09.github.io/project/loan/)
  -  This article provides an overview of HELOC loans and the challenges financial institutions face in assessing credit risk. The resource details the use of machine learning methods for predicting loan repayment. It covers crucial aspects of the modeling process, including data preprocessing, handling of missing values, and feature engineering. The document discusses various classification models, including logistic regression and random forests, and emphasizes the importance of model interpretability in the financial sector. Additionally, it highlights the use of metrics like recall and accuracy for model evaluation, particularly relevant for credit risk assessment. The resource also describes the development of an interactive interface for model predictions and explanations, which could be valuable for practical implementation of the credit scoring model. 
- [Scorecard Monitoring Tutorial](https://gnpalencia.org/optbinning/tutorials/tutorial_scorecard_monitoring.html)
    - The resource demonstrates high relevance to the loan repayment prediction project by utilizing the identical HELOC dataset for credit risk assessment and focusing on binary classification. It showcases scorecard modeling, a common approach in the financial industry, while covering crucial aspects such as feature selection and binning to enhance model interpretability. The tutorial illustrates data splitting for proper model evaluation and addresses the handling of special codes often encountered in financial data. Additionally, it mentions scorecard monitoring for maintaining performance over time and employs logistic regression, an interpretable model widely used in credit scoring. These elements collectively provide a comprehensive foundation for developing a classification model to determine customer loan repayment likelihood using the HELOC dataset.
- [FICO Website - HELOC Dataset Information](https://community.fico.com/s/explainable-machine-learning-challenge?tabset-158d9=d157e)
  - The FICO website provides necessary context about the dataset's structure, explains special values and cryptic variable names, and defines credit related terms. The FAQ clarifies important features and the dataset's composition, which is crucial for proper data preprocessing and interpretation. Additionally, it outlines the prediction task and target variable. This information is vital for accurate data handling, feature engineering, and model development in credit risk assessment.

## Data Description
The dataset used for this project is the Huggingface HELOC dataset from FICO. The sample includes 10,459 instances with each row representing a customer's loan application details and their classification label. The data was collected over a two year period and a stratified random sample was constructed out of a total of 242,000 customer accounts. Of those 10,459 instances, the distribution of "good accounts" to "bad accounts" is right around 50%. According to FICO, only 5,459 accounts made a seriously late payment during the collection window and all those accounts have been labeled as bad accounts. 

The anonymized dataset was obtained from the [Huggingface API](https://huggingface.co/datasets/mstz/heloc) and was prepared by FICO. It contains a comprehensive look into the credit attributes of customers looking to obtain a home equity line of credit (HELOC) in the amount of $5,000 - $150,000 and whether they will repay it within a 2 year time period. 

## Resources
- [EDA Notebook](https://github.com/samanthajmichael/dsba6211-summer2024--project/blob/main/01_exploratory.ipynb)
- [Modeling Notebook](https://github.com/samanthajmichael/dsba6211-summer2024--project/blob/main/02_modeling.ipynb)
