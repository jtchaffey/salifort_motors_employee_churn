# salifort_motors_employee_churn
Predictive model of employee churn for Salifort Motors, carried out as a project in the Google Advanced Data Analytics Certification course by Google on Coursera.

This project was initially conducted using Jupyter Notebooks as part of the Google Advanced Data Analytics curriculum, and is a copy of that notebook incorporating my own personal work.

**Overview**

This project utilized data supplied by the human resources department of Salifort Motors about employee attributes to create a machine learning model to predict whether employees would leave the company or not, aiming to reduce churn as a means to reduce the costs of training new employees. Both logistic regression models and tree-based learning models were constructed for evaluation in their application to the business goals, with small differences in scoring metrics between the two types. Through evaluation the model using random-forest methods was found to have a higher AUC score and selected as the champion model to proceed with. This model had an AUC score of 93.84% and F1 score of 88.67%.

An investigation of feature importances in the predictive models revealed the features with the greatest influence on an employee churning or not to be the employee's last evaluation score, the number of projects they were involved in, their tenure with Salifort Motors, and whether an employee was working a high number of hours per month on average. These features were identified as key attributes in both the decision-tree models and random-forest models.

**Business Understanding**

The use of a well-performing predictive model for employee retention/churn would financially help Salifort Motors by keeping their current employees and preventing extra expenses on finding and training new employees. The models and ranking of feature importances establish the idea that employees at Salifort Motors are currently being overworked, which goes on to directly influence employee churn at the company. Employees working on a high amount of projects, working a high amount of hours per month, and having previous negative evaluations were all factors which increased employee churn, and should be addressed.

**Data Understanding**

Data from the Salifort Motors human resources department included data on close to 15,000 employees and 10 features. These features included a self-rated satisfaction level at the company in addition to the most recent employee evaluation score, the average number of monthly work hours, whether an employee was promoted within the last 5 years, and whether an employee had left the company or not. Feature engineering was used to improve the consistency of feature names in the dataset, with additional feature engineering not felt to be necessary to carry out analysis.

**Modeling Evaluation**

The final model for a logistic regression approach achieved scoring metrics of 79% for precision, 82% for recall, an f1-score of 80% (based on weighted averages), and accuracy of 82% when used with the test data.

Random-forest models produced greater AUC scores and comparable scoring metrics to decision tree models both before and after feature engineering. When the test data was used, a random forest model using feature engineering produced an AUC score of 93.8%, precision score of 87%, recall of 90.4%, f1-score of 88.7%, and accuracy of 96.2%. Because of the higher-value scoring metrics obtained from the tree-based models, the random-forest model should be selected as the champion model for use by the human resources department to predict employee churn. 

**Conclusion**

The scoring metrics achieved by the random-forest model signify that the model should perform well with its predictions. The four identified key feature importances should be addressed by company culture at Salifort Motors to reduce employee churn. While tenure is a feature that cannot truly be influenced, the three other key features identified in the analysis should be improved if the matter of employee churn rates is to be addressed.
