## **1. Background**
     *  Recently, there has been an increase in employees leaving the company, prompting an examination of factors within the company that may contribute to employee attrition.
  
## **2. Data**
     *  The dependent variable is set as "attrition," indicating whether an employee has left or not, and independent variables such as "DistanceFromHome," "MonthlyIncome," "EnvironmentSatisfaction," and "PerformanceRating" are analyzed for their relevance to attrition.


## **3. Analysis** 
     *  General statistical analysis, correlation analysis, and machine learning predictive models are utilized.

#####   * General Statistical Analysis
     *   Analysis using histograms revealed that out of a total dataset of 1,470 individuals, 237 had left the company ("Yes" for attrition), while 1,233 had not ("No").
     *   Comparison using bar graphs showed that among those who left, although satisfaction with work and performance were high, factors contributing to attrition appeared to be distance from home and monthly income.
     *   When compared to those who didn't leave, the average distance from home was approximately 2km greater for those who left, and their monthly income was around $2,000 lower.
  
#####   *  Correlation Analysis
     *   Correlation analysis revealed strong correlations for those who left: "DistanceFromHome" with a salary increase percentage ("PercentSalaryHike") of 0.137674, "MonthlyIncome" with "JobLevel" at 0.945540, "EnvironmentSatisfaction" with "YearsSinceLastPromotion" at 0.104580, and "PerformanceRating" with "PercentSalaryHike" at 0.795337.
     *   However, as correlation analysis alone cannot determine causality between independent variables and the dependent variable of attrition, logistic regression was further employed.
  
#####  * Machine Learning Predictive Analysis
     *  Logistic regression predictive models along with a similar Random Forest were analyzed.
     *  Both models had an accuracy of over 0.5, indicating better than random guessing, but appeared similar. To determine which model is superior, ROC curves were plotted, and comparing the accuracies of the two models, the logistic model had a slightly higher accuracy at 0.86, but with similar AUC sizes. However, the Random Forest showed a higher score, suggesting better performance.

## **4. Results**    
    *   Examining the Random Forest variable importance, it showed that "MonthlyIncome" > "DistanceFromHome" > "EnvironmentSatisfaction" >"PerformanceRating" had significant influences, with income disparity among employees having the most significant impact. To reduce the number of employees leaving the company, attention should be paid to their monthly income.
    *   Additionally, when analyzing factors such as "YearsInCurrentRole", "YearsAtCompany" and "YearsWithCurrManager", "YearsAtCompany" was found to influence attrition. However, when compared with "DistanceFromHome", "MonthlyIncome", "EnvironmentSatisfaction" and performance, monthly income emerged as the most critical factor.    
    *   Therefore, the main trigger for attrition can be seen as monthly income. Given that satisfaction with work environment and performance among departing employees is high, strategies to increase employees' actual income, including performance-based bonuses and incentives, need to be explored.

## **5. Expected Impact**
    *  Identification of factors contributing to employee attrition and prevention of human capital outflow.

