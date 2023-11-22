
# Applied Data Analytics

## Wedge Project

I ended up having to accept a B for this assignment, try as I might I couldn't figure out the data cleaning after many, many solid attempts.

### Task 1

* Files for this task: 
Part-1-Uploading.ipynb


`Part-1-Uploading`: 

Uploading the cleaned wedge transaction data to GBQ




### Task 2

* Files for this task: 
Part-2-Sampling.ipynb
query_results.csv


`Part-2-Sampling`: 

This file takes a sample of 500 rows from the wedge transactions dataset and saves it to a csv file called 'query_results.csv'

`query_results`:
a sample of 500 random rows from the wedge transaction dataset	

### Task 3

* Files for this task: 
Part-3-Summary-Tables.ipynb
reporting.db


`Part-3-Summary`: 
This file holds 3 SQL queries that are run through GBQ and then creates a local database from the data pulled.

`reporting.db`:
This file is the database created in Part-3-Summary
<!--  Repeat for each file  --> 


## Query Comparison Results

Fill in the following table with the results from the 
queries contained in `gbq_assessment_query.sql`. You only
need to fill in relative difference on the rows where it applies. 
When calculating relative difference, use the formula 
` (your_results - john_results)/john_results)`. 



|  Query  |  Your Results  |  John's Results | Difference | Rel. Diff | 
|---|---|---|---|---|
| Total Rows  | 85760139  | 85760139  | 0  | 0  |
| January 2012 Rows  | 1070907  | 1070907  | 0 | 0  |
| October 2012 Rows  | 1042287  | 1042287   | 0  | 0 |
| Month with Fewest  | Feb  | Feb  | Yes/No  | NA  |
| Num Rows in Month with Fewest  | 6556770  | 6556770 | 0  | 0  |
| Month with Most  | May  | May  | No  | NA  |
| Num Rows in Month with Most  | 7578372   | 7578372  | 0  | 0  |
| Null_TS  | 7123792  | 7123792  | 0  | 0  |
| Null_DT  | 0  | 0  | 0  | 0  |
| Null_Local  | 234843  | 234843  | 0  | 0  |
| Null_CN  | 0  | 0  | 0  | 0  |
| Num 5 on High Volume Cards  | 14987.0  | 14987.0  | No  | NA  |
|  Num Rows for Number 5 | 460630   | 460630  | 0  | 0  |
| Num Rows for 18736  | 12153  | 12153  | 0  | 0  |
| Product with Most Rows  | banana organic  | banana organic  | No  | NA  |
| Num Rows for that Product  | 908639  | 908639  | 0  | 0  |
| Product with Fourth-Most Rows  | avocado hass organic  | avocado hass organic  | No  | NA  |
| Num Rows for that Product  | 456771  | 456771  | 0  | 0  |
| Num Single Record Products  | 2769   | 2769  | 0  | 0  |
| Year with Highest Portion of Owner Rows  | 2014  | 2014  | No  | NA |
| Fraction of Rows from Owners in that Year  | 0.7591   | 0.7591  | 0  | 0  |
| Year with Lowest Portion of Owner Rows  | 2011  | 2011  | No  | NA |
| Fraction of Rows from Owners in that Year  | 0.7372  | 0.7372  | 0  | 0  |

## Reflections

I gave it all I could trying to figure out the cleaning portion, I spent two full days doing nothing but trying to figure it out. I was just running into issues with the "\N"'s and the data types at the end. I feel like I did learn a ton about processing data as a whole. I think if I would have ask for your help, I probably could have figured out the cleaning portion but I wanted to test myself and see if I could figure things out. All in all, it's a good assignment for people to learn more about engineering, which isn't often focused on in the MSBA program.
