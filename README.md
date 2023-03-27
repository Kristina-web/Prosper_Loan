# (Prosper Loan dataset)
## by Kristina


## Dataset

The Prosper loan dataset contains information on thousands of loans issued by Prosper, a peer-to-peer lending marketplace that connects borrowers with investors. This dataset provides a valuable opportunity to explore trends and patterns in loan data, including factors that contribute to loan performance and borrower characteristics that affect loan outcomes.

In this analysis, we will use Python and a variety of data visualization and analysis tools to explore the dataset and gain insights into the factors that influence loan outcomes. We will start by cleaning and preprocessing the data, removing missing values and transforming variables as needed. We will then use descriptive statistics and visualization techniques to explore the relationships between loan attributes, borrower characteristics, and loan performance.

Our goal is to identify key factors that contribute to loan success or failure and to develop a predictive model that can be used to estimate the likelihood of loan default or other negative outcomes. By analyzing the Prosper loan dataset, we can gain valuable insights into the dynamics of peer-to-peer lending and develop strategies for improving loan performance and minimizing risk.

Resulting dataFrame consists of 113066 row and 25 columns

Here we checked for duplicates, a quick summary of our dataset, to get an idea of the overall distribution of datatypes, null values and the datatypes of our columns

    * Remove empty values
    * Left only importans columns (information features)
    * incorrect data in the columt of listingcreationdate - needed datatime
    * Not employed people in IncomeRange replaced with 0 (as they dont have income)
    * delete duplicates (to be sure even if it was shown 0)


## Summary of Findings

>The distribution of Borrower APR in the Prosper loan dataset shows multiple peaks at approximately 0.09, 0.18, 0.2, and 0.3. There is also a sharp peak around 0.35. Overall, Borrower APR has a multimodal distribution. Borrower APR values less 0.05 and above 0.4 are rare in the given dataset. If look briefly at the priority categorical distribution, it can be seen that three types prevail: completed, current and chargedoff.
>The are pikes in frequency at 5k, 10k, 15k, 20k and 25k, what means that most of the loans were given as n*5k.
>Here we can mark 3 most destributed ranges as C, D, B and the least NC. It can be interpreted that most of the borrowers have average to above-average creditworthiness based on the lender's evaluation. This suggests that the lender is likely to have lower risk of loan defaults, as they are lending to borrowers who have a good credit history and are considered less risky.
>The second histogram has right skewed view with the peak at 0.2. It means that there are more borrowers with a lower debt-to-income ratio and fewer borrowers with a higher debt-to-income ratio. This suggests that most borrowers have a relatively low amount of debt compared to their income, while a smaller number of borrowers have a higher level of debt relative to their income.
>The most amount of loans are spread among employed people and full-time. The least spreding almost even between part-time, not employed and retired, that not suprisingly as these people dosnt have clear income.
>The least of the borrowers are students, when the most is Professionals and Other representatives. The ratings of the most of the borrowers are from A to D (makin a bell-distribution)
>The number of listings has been consistently increasing over the years till 2013. However, it's important to note that the data only goes up until 11th March, 2014, which may explain the lower number of listings for that year as the data was collected before the year had elapsed.
The frequency of loan requests per day shows a relatively consistent pattern, with a slight decrease in the end of each month. There is a seasonal pattern in the loan requests, with higher demand during the first two months of the year (January to February) and the last few months of the year (September to December). This trend could be due to the holiday season or other seasonal expenses.
>Based on the information provided, it appears that the majority of borrowers in the dataset have monthly incomes in the range of 0-10000K, with the most common income levels being 5000k, 6000k, and 10000k per month. Beyond an income of 30000k per month, the distribution of borrowers becomes less even, suggesting that high-income borrowers are less common in the dataset. Understanding the income levels of borrowers can be helpful in identifying any patterns or trends related to borrower income, and may also inform lending decisions and risk assessment strategies.
>The data suggests that most listings in the dataset are associated with borrowers earning between 25,000 and 74,999 US dollars per annum, indicating a commonly observed income bracket. This information is useful for understanding borrower income levels and identifying potential patterns or trends in the data. It may also inform lending strategies and risk assessment analyses.
>The available data indicates that the state of California has the largest number of borrowers on the listings, with over 10,000 loan listings in the dataset. Other states such as Florida, New York, Texas, and Illinois also have a similar number of listings, indicating a comparable level of borrowing activity in these regions. In contrast, the states of Maine and North Dakota have the smallest number of listings by borrowers close to 0. This information provides insights into the geographical distribution of borrowers and can be useful for lenders and investors in developing lending strategies and identifying potential markets for loan offerings.
>The plot and regression analysis indicate a statistically significant negative correlation between LoanOriginalAmount and BorrowerAPR. The observed trend supports the notion that smaller loans tend to have higher interest rates, which can be attributed to fixed costs associated with loan processing and origination. On the other hand, larger loans may have slightly lower interest rates due to the economies of scale that come with higher loan amounts. This finding has important implications for lenders and borrowers, as it suggests that loan size should be carefully considered when evaluating the cost-effectiveness of different loan products. Overall, the observed relationship between loan size and interest rates highlights the need for nuanced and data-driven approaches to loan pricing and risk assessment.


## Key Insights for Presentation

> The first important insight for a presentation from the text is that the Borrower APR has a multimodal distribution, and the majority of borrowers have average to above-average creditworthiness based on the lender's evaluation. This suggests that the lender is likely to have lower risk of loan defaults, as they are lending to borrowers who have a good credit history and are considered less risky.

>The second important insight for a presentation is that there is a statistically significant negative correlation between LoanOriginalAmount and BorrowerAPR. This implies that smaller loans tend to have higher interest rates, which can be attributed to fixed costs associated with loan processing and origination. On the other hand, larger loans may have slightly lower interest rates due to the economies of scale that come with higher loan amounts. This finding has important implications for lenders and borrowers, as it suggests that loan size should be carefully considered when evaluating the cost-effectiveness of different loan products.