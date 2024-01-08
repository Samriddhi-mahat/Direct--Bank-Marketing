**Direct Bank Marketing:**
 The data in this project is related to direct marketing campaigns of a Portuguese banking institution. The marketing campaigns were based on direct phone calls to convince customers to open a deposit account. 

Objective: To build a predictive model to help the bank in their next marketing campaign

**Exploratory Data Analysis:**
                                   **Patterns and Insights:**
                                   
    - Students followed by retired followed by unemployed are more likely to open a deposit subscription account.
    - Single individuals are most likely to open a deposit subscription account.
    - Those with a higher education are more likely to open a deposit account.
    - Customers with credit default are less likely to open a deposit account compared with no credit default customers.
    - Customers with no housing loan are more likely to open a deposit account.
    - Customers with no personal loan are twice as likely to open a deposit account compared to customers with personal loan.
    - There is higher success rate when customers are contacted to their cell phone or telephone number.
    - There is more than 40% success rate in the months of March, December, September and October.
    - Customers with previous deposit account openings are more likely to open new accounts.
    - Students that are just entering college and/or getting jobs out of high school are more likely to open deposit accounts.
    - People over the age of 60 tend to open deposit accounts more.
    - People with almost no balance are more likely to open deposit accounts.
    - When call duration exceeds about 4 minutes, the probability of success decreases.
    - People who don’t subscribe in the previous contact are likely to subscribe if contacted a few more times.
    - As the number of contact days a customer was last contacted increases, the success probability decreases.

**Predictive Models:**                 Accuracy              Precision         Recall
- Logistic Regression                    90%                    34%              64%
- Logistic Regression (No Outliers)      95%                    17%              54%
- Decision Tree                          90%                    33%              62%
- Decision Tree (No Outliers)            95%                     9%              78%
- Random Forest                          91% (Overfitted)       68%              40%
- Random Forest (No Outliers)            95% (Overfitted)       69%              16%

Based on the accuracy metric, I recommend using either the Logistic Regression Model with no outliers or 
Decision Tree (no outliers) with maximum depth of 4. Both of the models have accuarcy of 95% for both 
training and validation dataset and hence prevents the overfitting or underfitting.
