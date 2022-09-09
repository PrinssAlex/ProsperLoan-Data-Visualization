
# ProsperLoan: Top Borrowers and Their Unique Characteristics
## by Prince A. Ogbodum

![project image](project_image.jpg)


# Dataset
 **Name of Dataset:** Loan Data From ProsperLoan 
 **Description of Dataset:** <br/>  
This data set contains 113,937 loans with 81 variables on each loan, including loan amount, 
borrower rate (or interest rate), current loan status, borrower income, and many others.

# Summary of Findings
- Most loans were taken by full-time working professionals, while students especially those in their early years in college took the least.
- Between 2006 - 2014, the highest number of loans received were recorded between October, 2013 to February, 2014.
- From 2006 to 2014, there was drought in loan funding in the year 2009. Then from 2011, there was an uptrend which experienced an initial slight dip in 2013 before moving upwards to an all time high through to 2014.
- Computer Programmers are the known professionals with the most funding.
- The average monthly income for the top occupation category is about USD7500.
- The category 1 and 12 which represent; debt consolidation and green loans respectively holds the position as the category with the highest and lowest count.
- The top 5 categories for computer programmers that got the most funding starting from the first to the fifth are; 'debt consolidation' (1), 'not available' i.e not stated by the borrower (0), 'other' i.e borrower's option not among those available (7), 'business' (3), and 'home improvement' (2).
- Most borrowers were most likely indebted to other loan lenders before taking this loan judging by the fact that the majority of loans listed were for debt consolidation.
- A good number of top borrowers are past due their payment date by at least 120 days.
- Computer programmer can be seen to have good employment statistics, the majority employed happen to be living in debt with over 6000 currently servicing a loan.
- The majority of workers who had worked the most number of months (>700) had no recommendation.
- While those with the highest score change at the time of listing belonged to a group.
- Belonging to a group may not be a strong factor in getting a loan but it does have a relationship with positive score change at the time of lisitng.

# Key Insights for Presentation
For most people taking a loan is not a good idea. However, When it comes to finances no one has the master key; 'money comes and goes' like 
someone once said. So, even though they may not like it, when faced with financial difficulty most persons will have no choice than to resort to taking loans to keep their head above water. 
    In this report, I visually analyzed the data set gotten from the US peer-to-peer loan company - Prosper Loan, between the year 2006 - 2013. To find out those unique characteristics associated with the borrowers who had the most fundings.
    
#### Preliminary Data Wrangling
After downloading the data set via python's requests library from Amazon cloud server, I did a brief visual and programmatic assessment
to verify the data set's quality and tidiness. Issues I discovered and fixed incuded:
    - Rename ListingCategory (numeric), to ListingCategory
    - Change ListingCreationDate data type from object(string) to datatime.
      Drop duplicate rows.
    - Fix missing values in the following columns (Occupation, DebtToIncomeRatio, GroupKey, ScorexChangeAtTimeOfListing,  
      BorrowerState, EmploymentStatus, and EmploymentStatusDuration).
    - Assign values greater than 10.00 in DebtToIncomeRatio column to 10.00.
    
#### Exploration
Afterwards, I did a series of visualizations including univariate, bivariate, and multivariate on the following variables:
    - ListingKey                   
    - Occupation                    
    - DebtToIncomeRatio            
    - CurrentlyInGroup                
    - ScorexChangeAtTimeOfListing  
    - Recommendations                
    - EmploymentStatus              
    - EmploymentStatusDuration     
    - LoanStatus                    
    - ListingCategory (numeric)     
    - StatedMonthlyIncome          
    - IncomeVerifiable                
    - IncomeRange                   
    - ListingCreationDate  
    
#### Insights
The following insights were gotten from my exploration analysis:
From 2006 to 2014, individuals from several walks of life requested loan to fund one financial obligation or the other. A distribution of the years with respect to loan listings shows that there was a slow but progressive increase from 2006 to 2008 when the first significant 
dip was experienced. Then in 2009, there was a major dip, a drought as a matter of fact. I assume this was due to the recession going on at the time (The Great Recession, 2007 - 2009). Plus, 2009, was the year that had the peak unemployment rate (10% in October). I believe the reason for this is that given the circumstances, many lenders were unwilling to give out funds at this time as this could cause them to become financial vulnerable and susceptible to loans since ProsperLoan is a peer-to-peer loan company. 
    
Furthermore, the majority of borrowers were employed professionals with computer programmers being at the top of list for professionals whose occupation were obtainable. Most of the loans obtained by these professionals were used for debt consolidation. With an average monthly income of $7500, and the possibility of having a family and several bills to pay, it is possible they were living off loans during the recession period and needed to take these loans to stay afloat.
    
The multivariate scatter plot showed that recommendations doesn't increase one's chance of being employed or getting a loan. However, most borrowers whose loan status read 'completed' had a long employment duration especially for computer programmers. Therefore, a lender is more likely to fund a loan if the borrower have a good number of employment duration compared to recommendations. 
    
