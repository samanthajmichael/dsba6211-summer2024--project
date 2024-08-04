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
- [Scorecard Monitoring Tutorial](https://gnpalencia.org/optbinning/tutorials/tutorial_scorecard_monitoring.html)
- [FICO Website - HELOC Dataset Information](https://community.fico.com/s/explainable-machine-learning-challenge?tabset-158d9=d157e)

## Data Description
The dataset used for this project is the Huggingface HELOC dataset from FICO. The sample includes 10,459 instances with each row representing a customer's loan application details and their classification label. The data was collected over a two year period and a stratified random sample was constructed out of a total of 242,000 customer accounts. Of those 10,459 instances, the distribution of "good accounts" to "bad accounts" is right around 50%. According to FICO, only 5,459 accounts made a seriously late payment during the collection window and all those accounts have been labeled as bad accounts. 

The anonymized dataset was obtained from the [Huggingface API](https://huggingface.co/datasets/mstz/heloc) and was prepared by FICO. It contains a comprehensive look into the credit attributes of customers looking to obtain a home equity line of credit (HELOC) in the amount of $5,000 - $150,000 and whether they will repay it within a 2 year time period. 
