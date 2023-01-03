# Lending Club
Lending club is an online loan market platform, facilitating personal loans, business loans and loans for medical purposes. The objective of this case study is to identify the risky applicants who are likely to default and there by minimize the financial loss to the company by analyzing the past data through Exploratory data analysis(EDA).

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

## General Information

The case study helps you in developing a basic understanding of risk analytics in banking and financial services and understand how data is used to minimize the risk of losing money while lending to customers. When a consumer finance company receives a loan application, the company has to make a decision for loan approval based on the applicant’s profile. Two types of risks are associated with the company's decision.
  1. If applicant is likely to repay the loan, then not approving the loan will lead to loss of business to the company.
  2. If applicant is likely to default the loan, then giving loan will result in financial loss to the company.

When a customer applies for a loan, the company can the following two decisions based on the candidate profile.
  1. Loan accepted: If the company approves the loan, then there are 3 possible scenarios as described below:
  
    a. Fully paid: The loan tenure is completed and customer has fully paid the loan (Prinicpal and interest)
    b. Current: Applicant is paying the installments and loan tenure is not completed. These candidates are not labelled as 'defaulted'.
    c. Charged-Off:  Applicant has not paid the instalments in due time for a long period of time, i.e. he/she has defaulted on the loan.
    
  2. Loan rejected: The company had rejected the loan after evaluating the candidate profile. Since loan is rejected, there is no transactional history of those applicants and hence data is not available with company.

## Conclusions(Refer the Notebook/PDF for the order)
1. There is a steady increase in the issuance of loan
2. It is clear that 60 Lakhs as the annual income is an outlier as most people annual income fall between 0-2 Lakhs as we see in the previous graph
3. 14.2% persons are labelled as 'Charged Off'
4. Most people opted for 36 years as their loan term
5. People with Annual income below 2 lakhs have taken more loans
6. People with Employment Length > 10 years have taken more loan
7. People have 7%-12% of rate of interest have opted more loans
8. Most people who opted for loan didnt make any enquiries or only less number of enquiries.
9. People who has RENT or MORTGAGE takes loan
10. Maximum loans were provided without verification
11. Pepole get loans more for the category 'debt_consolidation'
12. People in 'CA' have taken more loans
13. Correlation between variable that are observed on heatmap
14. loan amount, funded amount,funded_amnt_inv and installments show high correlation amongst each other, hence any one column can be taken for consideration for analysis.
15. total_payment,total payment_inv,total_rec_prncp and total_rec_int exhibit the same feature.
16. pub_rec_bankruptcy and pub_rec show 100% correlation.
17. recoveries and collection_recovery show a high correlation of 80% hence one of them can be discarded.
18. current applicants show a high correlation to out_prncp and out_prncp_inv
19. From the graph - 'Charged off persons - Term Frequency', In both 36 months and 60 months, persons who are labelled as 'Charged Off' are available.
20. On comparing the term ratio (Number of persons who opt for loan in 36 months to 60 months) for the entire dataset with the charged off dataset is 2.739 and 1.344. Both the ratio are not almost equal and that gives us the interesting pattern.
21. Visually we can see from two graphs that, at 60 months, there is a raise in the second graph. It implies, defaulters are available in both terms. But for the term 60 months, more defaulters are found even though the entire dataset has less number of persons who opted for 60 months
22. It is evident from the graph that, probability of the frequency of the people who charged off are those who are less than a year experienced
23. We cannot count in 10+ experienced. Why? - As the frequency of the loan is more for 10+ experienced people, charge off count is more. With respect to the ratio of "ChargeOff/Total", person whose employment <1 year tends to be a defaulter
24. From the graph on 'Annual Inc Vs Total Late fee (Mean)', it is known that people whose income falls between 1 Lakh - 4 Lakh and those who avail late fee tends to be a defaulter more.
25. As the Grade increases, the probability of charge off is also increased.
26. People who stated 'OTHER' as their Home ownership tend to charge off more.
27. Next to 'OTHER', people who stated 'RENT' as their ownership tend to charge off more

## Technologies Used
- Python
- pandas
- numpy
- metaplotlib
- seaborn

## Acknowledgements
Give credit here.
- This project was inspired by sajan kedia
- References Lhttps://github.com/sajankedia/LendingClubCaseStudy

## Contact
Created by **ganesh babu g** and **Pravin Pasi**  - feel free to contact us!
