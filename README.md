# Vivendo Food Claim Analysis

## Company Background
Vivendo is a fast-food chain in Brazil with over 200 outlets. As with many fast-food establishments,
customers make claims against the company. For example, they blame Vivendo for suspected food
poisoning. The legal team, who processes these claims, is currently split across four locations. The new head of the
legal department wants to see if there are differences in the time it takes to close claims across the
locations.

# Problem Statement
The head of the legal department wants a report on how each location differs in the time it takes to close claims.

# BUSINESS GOAL
The legal team wants to improve how long it takes to close claim acroo different locations

# Tools: Excel and Power Query
The dataset was analyze using the following steps
# Data Importation
The dataset was loaded into excel worksheet using power query
## Data Description
- Claim ID Character: this a unique identifier of the claim.
- Time to Close Numeric: number of days it took for the claim to be closed.
- Claim Amount: The claim value in the currency of Brazil.
- Amount Paid: Total amount paid after the claim closed in the currency of Brazil.
- Location: location of the claim which include “RECIFE”, “SAO LUIS”, “FORTALEZA”, or “NATAL”.
- Individuals on Claim: number of individuals on this claim.
- Linked Cases: This shows whether the claim is linked with other cases, either TRUE or FALSE.
- Cause: The cause of the food poisoning injuries, ‘vegetable’, ‘meat’, or ‘unknown’.

# Data Exploration and Validation
I explore the dataset to gain understanding of the data;s characteristics and identify trends and pattern

# Data Cleaning
This is to ensured that the data is free from errors and ready for analysis.

### Steps: The following tasks was performed
1. Spelling check, no spelling error found.
2.  Check for duplicates, no duplicate found.
3.  	A year column created from the Claim_ID using the mid funtions  =MID(A2, 12, 4) 
5.  	An anomaly was found in column 2, row 60. I corrected the anomaly by removing the negative sign to ensure the dataset integrity and consistency for further analysis.This correction 
      ensures that all ‘Time to Close’ values are non-negative and reflect the actual time required to close claims.
6.  	The empty cells on the “Cause” column were replace with unknown (78 Unknown replacement).
7.  	Ensure all relevant columns are correctly formatted
   
# Data Analysis:This involved analysing the dataset to address the following questions
- How does the number of claims differ across locations?
- - What is the distribution of time to close claims?
- How does the average time to close claims differ by location?

 The analysis result is summerized below
-	The number of claims across location includes Sao Luis = 30, and Recife = 25,  Fortaleza = 22, Natal = 21
-	The distribution of time to close across location includes: Sao Luis = 30902 and Recife = 21517, Fortaleza = 17061, Natal =12204
-	The average time to close for each location includes Sao Luis = 1030, Recife = 861, Fortaleza = 776, Natal= 581
-	
# Insights:
- Natal has the highest number of claims and took the shortest time to close claims on average of 581. This indicate that Natal is the most efficient in terms of closing claims.
- Sao Luis take the longest time to close claims on average of 1030 days	.
- There is variability in the efficiency of the claim processing across locations.
- There are Outliers in the ‘Time to close’. This indicates exceptional cases, inefficiencies, errors or special circumstances, therefore further investigation should be carried out.


# Recommendations
To ensure efficiency in closing claims, the legal team need to do the following
1.	Detailed review of the processing procedure should be conducted to identify best practices.
2.	Standardize these practices across locations to improve efficiency
3.	Assess if additional resources are required to handle claims efficiently
4.	Implement claim management systems to streamline processes
5.	Regular review meetings should be established to track progress of implemented changes and ensure continuous improvement in claim processing times.




