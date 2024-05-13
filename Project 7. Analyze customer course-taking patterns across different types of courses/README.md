## **1. Background**
*   Analyzing five sets of customer-related data from 2015 to 2024 to devise strategies for preventing customer churn and maintaining retention.

## **2. Data**
*   Collecting data related to course orders, enrollments, refunds, customer information, and user details.
   - Using the following data files: order.csv, course.csv, refund.csv, customer.csv, user.csv.


## **3. Analysis** 

#####   *  (Order) The top 3 days with the highest sales and the bottom 3 days with the lowest sales in January 2022, along with the revenue (list_price), number of orders, number of customers, and number of courses
     *   Top 3 days with the highest sales:
     *  2022-01-03: ₩48,980,000, 2022-01-07: ₩34,700,000, 2022-01-05: ₩33,840,000
     *  Number of orders: 4,110, Number of customers: 6,598, Number of courses: 197

     *  Bottom 3 days with the lowest sales:
     *  2022-01-01: ₩6,260,000, 2022-01-22: ₩2,685,000, 2022-01-29: ₩8,920,000
     *  Number of orders: 806, Number of customers: 1350, Number of courses: 179

#####   *  (Order) Analyzing the discount rate for each course on a monthly basis
     *  Monthly discount rates for each course have been calculated, and among them, the course with the highest discount rate is '[내부용]Apach' with a discount rate of 200000.0.

#####   *  (Course) To analyze the most frequently mentioned words in the course keywords
     *   To find the most frequently mentioned words in the course keywords, we need to tokenize the 'keywords' column and identify the most commonly mentioned words.
     *   Although the most frequently mentioned word in the 'keywords' column appears as ',', which is not a word, we used code to find the second most frequently mentioned word. '평생소장' appeared 86 times, making it the most frequently mentioned word.

#####   *  (Refund) Analyzing the courses with the highest number of refunds
     *   The course ID with the highest number of refunds is 213368, and it had 269 refunds.
     
#####   *  (Customer) Analysis of the customer who has enrolled in the most courses and the amount spent
     *   The customer ID who enrolled in the most courses was 819532, and they spent a total of 6.69 million won.

#####   * (Order) Average course enrollment rate differs between weekends and weekdays
     *   It was observed that customers enroll in courses approximately three times more on weekdays compared to weekends
     *   Weekend course enrollment rate: 25.7%, Weekday course enrollment rate: 74.3%.

#####   *  (User) Analysis of the most active times for user registrations (created_at)
     *  The most active registration times by month were Jan, Feb, and Dec at 1 PM, Mar and Oct at 5 AM, Jun at 6 AM, and the other months (Apr, May, Jul, Aug, Sep, Nov) at 7 PM.

#####   *  (Order) Analyzing the frequency distribution table of course prices (list_price) in 50,000 won intervals
     *  The majority of courses, 267,266 in total, had prices below 50,000 won, and further divisions could be made up to less than 6,700,000 won

#####   *  (Order) Analysis of the Amount (list_price) and User Distribution for Completed, Pending, and Cancelled Courses by Month
     *  May was the month with the lowest order amount across all three categories.
     *  December had the highest order amount for both completed and pending courses, while January had the highest for cancelled courses.

#####   *  Trend analysis from January to December 2022
     *  (order) Comparison of monthly course prices (list_price) and sales prices (sale_price)
             Order data consisted only of 2022 data.
             When comparing the course price (list_price) and the sales price (sale_price), the difference between the two prices was                     largest in December (348,080,000 won) and smallest in June (57,600,000 won).
     *  (course) Monthly comparison of ongoing and pending courses
             Since course data was from 2018 to 2022, only 2022 data is filtered and analyzed
             As of 2022, it was found that there were more ongoing id than pending id
     *  (user) Period from registration to last login date
             As of 2022, it can be seen that USERs log in again when less than 50 days (approximately 46 days) have passed since their new                registration.
             The number of users who took up to 350 days to reconnect is very small, around 210
     *  (customer) Monthly user registration trend
             It can be seen that the highest number of registrations were in January with 9,332 users, followed by December with 8,587                    users. The month with the fewest registrations was May with 5,185 users.
             Overall, there was a decline from January to May, followed by an increase from May to August, but then another decline from                  August to November.
     *  (refund) Monthly analysis of the number of refunded courses and amounts
             REFUND data consists of records from January 3 to December 30, 2022, with the state being completed and the type being                       ADMIN_AUTO_REFUND.
             Refunds were most frequent in January and December, with amounts exceeding 2,300,000 KRW. The lowest month was March, with 774               courses refunded totaling 14,900,000 KRW.
             In contrast, October saw 906 courses refunded, but the total amount was lower at 14,990,000 KRW.

 ## **4. Conclusion**
    *   Customers tend to sign up around three times more on weekends than on weekdays.
    *   In December, there is a significant amount of orders for courses, but there is a notable difference between the actual course price and the selling price, leading to a high rate of refunds. While there is a high number of course registrations in January and February, there is also a high rate of refunds, especially in January.
    *   The peak period for member registrations was from December to February around 1 PM, while in other months, registrations were more active between 5 to 7 PM. Considering this pattern, strategies to encourage course attendance at different times of the day are necessary.
    *   Additionally, May consistently had the lowest order amounts across all statuses: completed, pending, and canceled. Understanding the reasons behind this and devising strategies to increase course purchase rates are necessary.

### **Advanced Analysis of the Project (Course Data) - Image**
<img width="404" alt="Project 3 visualization" src="https://github.com/Y-Junghye/Portfolio/assets/159558491/c3b019eb-6131-446c-a533-0564e82a217b">

      * The highest number of users, 541, had completed courses.
      * When dividing users by the type of courses or books attended, the overwhelming majority attended courses.
      * When analyzing total course hours, there was a high tendency, 43.5%, for users to listen to courses for over 10 hours.
      * Analyzing the signup trends by year, there was a decline in signups between 2018 and 2019, but from 2019 to 2021, there was an               increase of 7 to 90 signups per year, and from 2021 onwards, there was an increase of over 2.5 times.
      * Analysis of course keywords revealed that the keyword "평생소장 (lifelong ownership)" appeared the most, 722 times.
    
## **5. Expected Effects**
    *   The analysis of various types of data such as course orders, attendance, preferred days, etc., allows for understanding customer             patterns.
    *   Understanding the overall patterns of customers enables the formulation of strategies to reduce refund amounts, prevent churn to             other platforms, etc.


