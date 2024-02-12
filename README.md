# PyPoll with Python

## Overview of Project

### Background
In this module, we were able to help Tom and Seth by writing a Python program that...
1. Reads the data from the CSV file
2. Calculates various summary statistics and results, such as finding the winning candidate, based on the popular vote, AND...
3. Saves the results to our txt file

### Purpose
In the challenge, the election commission now requests three more pieces of data, this time, accounting for the county.

## Election-Audit Results
Note: all results can also be viewed in the txt file in the analysis folder.

- **Number of Votes Cast:** 369,711

- **Breakdown of Number of Votes & Percentage of Total Votes, for each County**
    * County: % of Total Votes (Number of Votes)
    * Jefferson: 10.5% (38,855)
    * Denver: 82.8% (306,055)
    * Arapahoe: 6.7% (24,801)

- **County with the Largest Number of Votes:** Denver

- **Breakdown of Number of Votes & Percentage of Total Votes, for each Candidate**
    * Candidate: % of Total Votes (Number of Votes)
    * Charles Casper Stockham: 23.0% (85,213)
    * Diana DeGette: 73.8% (272,892)
    * Raymon Anthony Doane: 3.1% (11,606)

- **Winning Candidate, Vote Count & Percentage of Total Votes**
    * Winner: Diana DeGette
    * Winning Vote Count: 272,892
    * Winning Percentage: 73.8%



## Election-Audit Summary
This script will work with ANY election, so long as the data is in the same format as our election_result.csv file. Specifically, we need the input data to have three columns: Ballot ID, County, and Candidate, preferably in this order, or else we'll have to make some small modifications to the script. Thus, for any election data that's in the same format as our CSV file, this script can instantly compute the exact same summary statistics and results. However, if we wanted to extract more data from a dataset of election results, we could modify the following. 

First, if necessary, we could determine the winner of the election using a method other than popular vote. For instance, take the traditional United States presidential election. We could add a dictionary with all 50 states as the keys and the number of electoral votes per state as the values. Then, we'd calculate the winning candidate IN EACH STATE, and assign that state's electoral votes to the corresponding candidate. Rinse and repeat, and we will have found a winner. 

Secondly, if our dataset came with more data (ie. more columns) we could compute other summary statistics. In one such case, we could compare male voter turnout to female voter turnout, or compare voter turnout based on any other category, such as age, race, etc. Furthermore, we could look for trends based on these provided categories, and potentially draw a connection such as "Most female voters voted for Diana DeGette, the only female candidate in the election."

In conclusion, there's truly no limit to what our script can do, with a few modifications.
