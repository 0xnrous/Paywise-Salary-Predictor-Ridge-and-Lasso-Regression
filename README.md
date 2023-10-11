# Paywise-Salary-Predictor-Ridge-and-Lasso-Regression
This Notebook aims to build linear regression models for the Hitters dataset while minimizing error scores across using Ridge and lasso Regression 



## Insights

After conducting a detailed analysis of the dataset and implementing Ridge and Lasso regression, several key insights and observations have emerged:

1. **Strong Linear Relationships:**
   - It's evident that specific baseball player statistics gathered across seasons, including 'CWalks,' 'CHmRun,' 'CAtBat,' 'CHits,' 'CRuns,' and 'CRBI,' have the strongest linear relationship with the 'Salary' target variable.


2. **Weak Predictive Variables:**
   - Approximately half of the variables exhibit weak relationships with 'Salary.' These variables, such as 'Division_W,' 'League_N,' 'NewLeague_N,' 'Errors,' 'Assists,' 'PutOuts,' 'HmRun,' and 'AtBat,' contribute minimally to salary predictions.

3. **Complexity and Feature Selection:**
   - Some variables introduce complexity to the model without significantly improving performance. A careful feature selection process is essential to address this issue.

4. **High Correlation Between Features:**
   - Strong correlations were observed between certain features, such as 'CRuns,' 'Years' (number of years spent in the major leagues), 'CHmRuns' (career home runs), and 'CHits' (career hits), indicating multicollinearity in the data.

5. **Model Performance and RMSE:**
   - The difference between actual and predicted values is noticeable, as reflected in the high Root Mean Square Error (RMSE) score, indicating that the model has room for improvement.

6. **Training vs. Testing Scores:**
   - The model's training score (approximately 56%) significantly outperforms the testing score (approximately 34%), suggesting the presence of multicollinearity issues or overfitting.

7. **Ridge Regression:**
   - Ridge regression outperforms simple Linear Regression in terms of RMSE, and its testing score (44.4%) surpasses the testing score of Linear Regression. A smaller tuning parameter in Ridge regression further enhances its performance.

8. **Lasso Regression:**
   - Lasso regression exhibits a similar trend as Ridge regression but achieves slightly lower performance according to scoring metrics.

9. **Feature Elimination:**
   - Both Ridge and Lasso regression effectively reduce the coefficients of some features to zero, indicating their ability to handle multicollinearity and select the most relevant features.

**Final Overview:**
   - In summary, Ridge and Lasso regression models prove to be more effective in handling the dataset compared to Linear Regression. These models address multicollinearity, enhance predictive performance, and provide valuable insights into feature selection and model improvement.

These insights can guide further model refinement and feature engineering, ultimately leading to more accurate salary predictions.
