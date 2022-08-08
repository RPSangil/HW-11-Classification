# HW-11-Classification
**Unit 11 - Risky Business**

## The Scenario

Mortgages, student and auto loans, and debt consolidation are just a few examples of credit and loans that people seek online. Peer-to-peer lending services such as Loans Canada and Mogo let investors loan people money without using a bank. However, because investors always want to mitigate risk, a client has asked that me to help them predict credit risk with machine learning techniques.

In this assignment I  have built and evaluated several machine learning models to predict credit risk using data you'd typically see from peer-to-peer lending services. Credit risk is an inherently imbalanced classification problem (the number of good loans is much larger than the number of at-risk loans), so I have needed to employ different techniques for training and evaluating models with imbalanced classes. I have uses the imbalanced-learn and Scikit-learn libraries to build and evaluate models using the two following techniques:

- <ins> Resampling </ins> - Resampling is a methodology of economically using a data sample to improve the accuracy and quantify the uncertainty of a population parameter.[<sup>1</sup>](reference-list)

- <ins> Ensemble Learning </ins> - Ensemble learning is a method where multiple models are combined into one powerful predictor. In classification instances, the different models might make a final prediction by calculating which class had the most votes or predictions. In regression instances,  the mean of all results is typically taken and then offered as the final prediction.

## Navigating the GitHub

The following was provided at the beginging of the assessment and can be found in the Starter_Code folder:

- [Lending Club Loans Data Resources](https://github.com/RPSangil/HW-11-Classification/tree/main/Starter_Code/Resources)
- [Ensemble Starter Notebook](https://github.com/RaelynSangil/HW-11-Classification/blob/3b69a2a713b8d65e74f65a68a7a9c1f8fb1b2784/Starter_Code/credit_risk_ensemble.ipynb)
- [Resampling Starter Notebook](https://github.com/RaelynSangil/HW-11-Classification/blob/3b69a2a713b8d65e74f65a68a7a9c1f8fb1b2784/Starter_Code/credit_risk_resampling.ipynb)

In the Worked_Code folder you will find:

- [Lending Club Loans Data Resources](https://github.com/RPSangil/HW-11-Classification/tree/main/Worked_Code/Resources)
- [Credit Risk Ensemble](https://github.com/RPSangil/HW-11-Classification/blob/5605cb4c12195659d62210815aa24768b8194796/Worked_Code/credit_risk_ensemble.ipynb) - The code I have written for this notebook.
- [Credit Risk Resampling](https://github.com/RPSangil/HW-11-Classification/blob/5605cb4c12195659d62210815aa24768b8194796/Worked_Code/credit_risk_resampling.ipynb) - The code I have written for this notebook.

## Questions and Answers

### Credit Risk Ensemble

1. Which model had the best balanced accuracy score?

    Between the two models the Balanced Accuracy Scores were:

    * Balanced Random Forest Classifier - Balanced Accuracy Score: 0.7887512850910909

    * Easy Ensemble Classifier - Balanced Accuracy Score:0.931601605553446

    
    The Easy Ensemble Classifier has a higher score, there for the best balanced accuracy score was Easy Ensemble Classifier - Balanced Accuracy Score:0.931601605553446.
    

2. Which model had the best recall score?

    Between the two models the recall scores were:

    * Balanced Random Forest Classifier - 0.87

    * Easy Ensemble Classifier - 0.94

    
    The Easy Ensemble Classifier has a higher score, there for the best recall score was Easy Ensemble Classifier - 0.94.
   
3. Which model had the best geometric mean score?

    Between the two models the geometric mean scores were:

    * Balanced Random Forest Classifier - 0.78

    * Easy Ensemble Classifier - 0.93
    
    The Easy Ensemble Classifier has a higher score, there for the best geometric mean score was Easy Ensemble Classifier - 0.93.

4. What are the top three features?

    Top three features are:

    * total_rec_prncp = 0.07876809003486353

    * total_pymnt = 0.05883806887524815

    * total_pymnt_inv = 0.05625613759225244

### Credit Risk Resampling

1. Which model had the best balanced accuracy score?

   Between the two models the balanced accuracy scores were:
   
   * Simple Logistic Regression- Balanced Accuracy Score: 0.9520479254722232

   * Naive Random Oversampling - Balanced Accuracy Score: 0.9934649587814939

   * SMOTE Oversampling - Balanced Accuracy Score: 0.9934649587814939

   * Cluster Centroids Undersampling - Balanced Accuracy Score: 0.9929503031930944

   * SMOTEENN Combination Sampling - Balanced Accuracy Score: 0.9934649587814939

   
   The were 3 models with the best balanced accuracy scores of 0.9934649587814939: Naive Random Oversampling, SMOTE Oversampling, SMOTEENN Combination Sampling.

2. Which model had the best recall score?

   Between the two models the recall scores were:
   
   * Simple Logistic Regression- recall score: 0.99

   * Naive Random Oversampling - recall score: 0.99

   * SMOTE Oversampling - recall score: 0.99

   * Cluster Centroids Undersampling - recall score: 0.99

   * SMOTEENN Combination Sampling - recall score: 0.99

   
   As all models had the same recall score they all scored equally well.

3. Which model had the best geometric mean score?

    Between the two models the geometric mean scores were:
   
   * Simple Logistic Regression- recall score: 0.95

   * Naive Random Oversampling - recall score: 0.99

   * SMOTE Oversampling - recall score: 0.99

   * Cluster Centroids Undersampling - recall score: 0.99

   * SMOTEENN Combination Sampling - recall score: 0.99

   
   Every model except the Sumple Logistic Regression Model scored a of 0.99. those models all scored equally well.


# Reference List
- [<sup>1</sup> https://machinelearningmastery.com/statistical-sampling-and-resampling/#:~:text=Resampling%20is%20a%20methodology%20of,of%20a%20nested%20resampling%20method.](https://machinelearningmastery.com/statistical-sampling-and-resampling/#:~:text=Resampling%20is%20a%20methodology%20of,of%20a%20nested%20resampling%20method.)
