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

### Steps:
- Spelling check, no spelling error found.
-	Check for duplicates, no duplicate found.
-	A year column created from the Claim_ID using the mid funtions
-	An anomaly was found in column 2, row 60. I corrected the anomaly by removing the negative sign to ensure the dataset integrity and consistency for further analysis.
  This correction ensures that all ‘Time to Close’ values are non-negative and reflect the actual time required to close claims.
-	The empty cells on the “Cause” column were replace with unknown (78 Unknown replacement).
-	Ensure all relevant columns are correctly formatted


