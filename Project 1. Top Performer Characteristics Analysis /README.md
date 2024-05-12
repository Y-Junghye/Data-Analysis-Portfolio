## **1. Background**
*   There is a growing trend of employees achieving outstanding performance within the company. Therefore, an analysis was conducted to identify the factors contributing to the emergence of high-performing employees within the organization.

## **2. Data**
*  The dependent variable was set as PerformanceRating, with independent variables focusing on factors closely related to performance, including the percentage increase in salary (PercentSalaryHike), years with current manager (YearsWithCurrManager), and years since last promotion (YearsSinceLastPromotion).

## **3. Analysis**
*  Utilizing descriptive statistics, correlation analysis, and regression models

    *  Descriptive Statistics:
       - A histogram analysis revealed that out of the total dataset of 1,470 individuals, 1,244 received a performance rating of 3, while 
         226 received a rating of 4.
       - Comparing performance ratings with the percentage increase in salary(PercentSalaryHike) showed that those with a rating of 4 had an
         average increase of 21.84%, whereas those with a rating of 3 had an average increase of 14.0%.
       - Years in the current role showed minimal difference between ratings 3 (average of 4.18 years) and 4 (average of 4.23 years).
         Similarly, there was little disparity in years since last promotion.
         Variables such as TotalWorkingYears, WorkLifeBalance, and StockOptionLevel exhibited similar performance ratings, suggesting
         minimal impact.

    *  Correlation Analysis:

       - PercentSalaryHike exhibited the strongest correlation (0.77) with performance rating.
       - Other variables showing positive correlations included YearsInCurrentRole (0.035), DistanceFromHome (0.027), YearsWithCurrManager
        (0.023), and YearsSinceLastPromotion (0.018).
       - However, correlation analysis alone cannot establish causality between independent variables and the dependent variable. 
         Therefore, regression analysis was further conducted.

    *  Regression Analysis:
       - Initial regression analysis yielded a coefficient of determination (R-squared) of 0.6, indicating moderate explanatory power. 
         Most variables exhibited p-values below 0.05, except for DistanceFromHome and YearsWithCurrManager.
       - Despite expectations of higher R-squared values, subsequent regression analysis excluding non-significant variables still yielded
         an R-squared of 0.6, with all variables showing significant p-values.
          + A 1% increase in PercentSalaryHike corresponded to a 0.0763-point increase in performance rating.
          + A one-year increase in YearsInCurrentRole or YearsSinceLastPromotion led to a 0.0024-point increase in performance rating.

## **4. Results**

    *  Through correlation and regression analysis, it was revealed that the percentage increase in salary significantly influences employee
       performance.
    *  Additional variables such as work-life balance, stock option level, and total working years were included in the regression analysis,
       but they showed non-significant p-values.
    *  Therefore, the pivotal factor in enhancing employee performance is the percentage increase in salary. While performance bonuses are
       important, increasing the percentage increase in salary requires a detailed understanding of individual performance to be reflected
       in performance evaluation processes.
  
## **5. Expected Effects**
    *  Based on the results, refining performance evaluation criteria to include more detailed assessments of current roles could increase
       both the percentage increase in salary and overall performance.
