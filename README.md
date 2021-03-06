# Peer-to-Peer-Lending-Analysis--Tableau-Application
## A Story about the Online Peer-to-Peer Loan Business
## Author: Shashwat Jyotishi 	
## Tableau Project: Data Analysis
 
### About:
Peer-to-Peer lending platform is the one that aims to connect people who need money with those who have the money to invest. In this data analysis project, I have explored the dataset and used Tableau to create my visualizations.

### Dataset:
The loan data set contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others. The data-dictionary can be found in this repository itself. 

### Summary:
In Peer-to-Peer lending, there are three main stakeholders: borrowers, lenders and the company itself. In my Tableau story, I have done exploration on the relationships between these people, what affects borrowers' Score and who defaults the most. 

Firstly, I have done a time series analysis ranging from year 2007 – 2014 about the number of loans taken by borrowers, the amount of their loans and how their Score got affected in this duration. I noticed that since 2009, the loan business increased and climbed up quickly since 2013 and then dropped down at beginning of 2014 while the borrower credit scores constantly dropping over this time. Some states had default rates of more than 30%.

![Screenshot (20)](https://user-images.githubusercontent.com/73714933/100597691-c19b8980-3323-11eb-9a1f-64946edfc693.png)


![Screenshot (21)](https://user-images.githubusercontent.com/73714933/100597695-c3654d00-3323-11eb-9a1a-c80e18ce21ed.png)


Then, I have explored the defaulters, reason for defaults, and reason for borrowers to take loans. I found out that the people with $0 income have highest default rates and most defaulters invest in the loan type ‘D’. 

![Screenshot (23)](https://user-images.githubusercontent.com/73714933/100600458-52c02f80-3327-11eb-9d98-7a634be9ac72.png)


![Screenshot (24)](https://user-images.githubusercontent.com/73714933/100600467-5489f300-3327-11eb-8c93-11cd529647d6.png)


![Screenshot (27)](https://user-images.githubusercontent.com/73714933/100600471-55bb2000-3327-11eb-918f-04006255774e.png)

Breaking down to occupation-wise category, an interesting pattern was found that the college students group ie; students who are enrolled in higher grade studies have more loans, higher borrowers and default rates. While this made sense with $0 income, the sophomore students were amongst the top defaulters and had lower number of loans. 

![Screenshot (29)](https://user-images.githubusercontent.com/73714933/100600473-5653b680-3327-11eb-9130-26ea5a37e3ad.png)


Lastly, I have looked at the incomes and losses on different loan ratings and inferred that the ‘HR’ loan rating had the highest loss, even though this type of loan is given to most credit-worthy borrowers. However, looking at the net principal returns over the time I noticed loans 'C' & 'D' had higher losses than other loans and are most risky.

![Screenshot (30)](https://user-images.githubusercontent.com/73714933/100602185-93b94380-3329-11eb-98a7-74e7c765745a.png)


### Design Decisions:

I first sifted through the dataset and gave a rough thought on which variables should I be interested in exploring and which were outside the domain of my exploration. I first planned on making another file which would contain the subset of variables that I want to explore. But, I instead decided to use the entire dataset, just in case I got any new ideas midway through my exploration.

I wanted my Tableau story to have a purpose, to show to those who are interested in facts about the loan data. My focus was on loan borrowers, their occupations and subsequent default rates, their incomes, and what kinds of loan were taken by the borrowers. I got a few amazing feedbacks like mapping state-wise default rate, including the borrowers purpose for loan and some minor spelling mistakes. All these have contributed in improving my visualizations.

•	I have used scatter plots to show how much loan amount on different listing categories have changed over the time.\
•	Line plots to show how much the Score of borrowers has changed over the time.\
•	Geo Maps to show the default rate in each state.\
•	For showing the state-wise map of Defaulters and loan trends over time, I have used Multi-select Legends and automatic color pallets because in the dashboard, I want users to be able to select multiple options and see thee corresponding effect in all the charts.\
•	For Bar Plots in Income and Credit Score dashboard, I have used radio button legends, so that users can see how different income groups affect the Score. Also, I used Color blind color palette based on feedback from Udacity review.\
•	In the final Estimate and Actual dashboard, I have removed the legends, since looking at the X and Y axis Rating(Alpha) is self-explanatory.

### Feedbacks:

After completing the first sketch of my Tableau story, I shared it on Udacity Slack group and emailed the link to two of my friends. I received few important feedbacks mentioned below:

##### •	Showing state-wise default rate –
For this, I created a new numerical variable called Default Rate from Loan Status and mapped with Borrower State, this showed an interesting finding that in states like CA, TX, NY, IL the default rates were quite high with CA having highest defaulters (>700).
##### •	Finding why people borrow money – 
This was a bit tricky. But from the data dictionary, I found a variable called Listing Category that had reasons for loans. I found out that since 2007 borrowers took most Personal loans which suddenly dropped in 2009. Then since 2009 the most loans borrowers took were for Home Improvement or Business which steadily kept increasing with steady-drop in borrowers’ credit ratings.
##### •	There were also some minor feedbacks on spelling, typos, grammar and chart changes.
##### •	I really appreciate all the feedback I got which helped me in improving my plots.
