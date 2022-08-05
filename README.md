# (ProsperLoan Data Exploration)
## by (Olatunji Jola)


## Dataset
The ProsperLoanData Dataset was put together by Prosper Funding LLC, The first peer to peer online loan company. The dataset contains 113937 observations and 81 variables about different loan listing from 2005 to 2014.
The listing can be broadly divided into three observational units, a concise summary of the loan listing, a detailed profile of the borrower and historical data of previous loan by the same borrower and information about the current loan.
a more detailed description of the dataset variables is available in the dataset variable defination [here](https://www.google.com/url?q=https://docs.google.com/spreadsheet/ccc?key%3D0AllIqIyvWZdadDd5NTlqZ1pBMHlsUjdrOTZHaVBuSlE%26usp%3Dsharing&sa=D&ust=1554484977407000).


## Summary of Findings

> In the exploration, I found that with increased BorrowerAPR comes increased Yield for the lender which comes at greater risk as well. and also that creditscore of the borrower is a base criteria for determining the level of risk exposure a lender will have in entering into a deal with any borrower.

Furthermore, CreditScore and BorrowerAPR varies with Employment Status and Occupation. With respect to occupation, creditscore varies in groups which can be easily identified with the level of skills required to perform each job. The occupations were therefore binned by their skill level to obtain more insight.
Exploring how the Employment status varies with borrowerAPR and Creditscore, I observed that the relationship between BorrowerAPR and EmploymentStatus can be generally divided into three by CreditScore value.
          
         - The lower CreditScore region (averagely CreditScore < 600): Associated with higher risk and higher BorrowerAPR. Here the OCcupationStatus and EmploymentStatus show differetiated borrowerAPR

        - The intermediate CreditScore region (ranging between 600 and 750): Associated with moderate Risk and Yield. The different levels of OccupationStatus and EmploymentStatus tend to converge at this region.

        - The higher CreditScore region (> 750): Associated with Lower BorrowerAPR, lower LenderYield and lower risk. Here also, the different levels of Employment status and OccupationStatus are differentiated by BorrowerAPR.

        - The homeownership status has the tendencies to reduce the differentiation between differnt level's BorrowerAPR while also extending the range of the CreditScore for each level more to the right.

Similar patterns can also be observed for Occupation status with respect to Credit Score and BorrowerAPR

## Key Insights for Presentation

For the presentation, I focus on how the BorrowerAPR values varies with CreditScore for EmploymentStatus and Occupation Status and the extra influence of homeownership on this relationship.

I started by introducing the borrowerAPR distribution. Then I show the relationship between BorrowerAPR, LenderYield and EstimatedLoss this shows that LenderYield increases with BorrowerAPR but so does EstimatedLoss. After that, I show the CreditScore distribution and the relationship between CreditScore and BorrowerAPR and as expected, BorrowerAPR reduces with CreditScore.

I go further to show the relationship between CreditScore, BorrowerAPR, EmploymentStatus, Occupation and IsBorrowerHomeowner.

Finally, I show how BorrowerAPR varies with EmploymentStatus and Creditscore and the influence of Homeownership status on this relationship. This same approach is employed to show how BorrowerAPR varies with Occupation and Creditscore and the influence of homeownership on the relationship.

I used different colors pallete for the different levels of EmploymentStatus and OccupationStatus to show that they are different between plots, I re-emphasised this difference by using different marker style.

I also used regressionlines to show the trend while using mean points at different creditscore value instead of a fullscatter plot to simplify the visualisation. 




