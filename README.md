# PyPoll with Python

## Overview of Project

### Background
In this module, we assisted Tom and Seth, two Colorado Board of Election employees, by writing a Python program that...
1. Read in election data from a CSV file
2. Calculated various summary statistics and results, such as determining the winning candidate, based on the popular vote, AND...
3. Saved an elections results report to a txt file

### Purpose
In the challenge, the election commission now requests three more pieces of data, this time, accounting for the county.

## Election-Audit Results
Note: all results can also be viewed in the txt file in the analysis folder.

- **Number of Votes Cast:** 369,711

- **Breakdown of Number of Votes & Percentage of Total Votes, for each County**
    * Jefferson: 38,855 (10.5%)
    * Denver: 306,055 (82.8%)
    * Arapahoe: 24,801 (6.7%)

- **County with the Largest Number of Votes:** Denver

- **Breakdown of Number of Votes & Percentage of Total Votes, for each Candidate**
    * Charles Casper Stockham: 85,213 (23.0%)
    * Diana DeGette: 272,892 (73.8%)
    * Raymon Anthony Doane: 11,606 (3.1%)

- **Winning Candidate, Vote Count & Percentage of Total Votes**
    * Winner: Diana DeGette
    * Winning Vote Count: 272,892
    * Winning Percentage: 73.8%


## Election-Audit Summary
This script will work with ANY election, so long as the data is in the same format as our election_result.csv file. Specifically, we need the input data to have three columns: Ballot ID, County, and Candidate, preferably in this order, or else we'll have to make some small modifications to the script. Thus, for any election data that's in the same format as our CSV file, this script can instantly compute the exact same summary statistics and results. However, if we wanted to extract more data from a dataset of election results, there are a few modifications we could make.

First, if necessary, we could determine the winner of the election using a method other than popular vote. For instance, using the United States presidential election as an example, we could create a dictionary with all 50 states as the keys and the number of electoral votes per state as the values. Then, we'd calculate the winning candidate in each state, and assign that state's electoral votes to the corresponding candidate, and whichever candidate receives the most electoral votes wins the elecion.

Secondly, if our dataset accounted for other variables, we could compute new summary statistics. In one such case, we could compare male voter turnout to female voter turnout, or compare voter turnout based on any other category, such as age, race, etc. Furthermore, we could look for trends based on these provided categories, and potentially draw a connection such as "Most female voters voted for Diana DeGette, the only female candidate in the election."

In conclusion, there's truly no limit to what our script can do, with a few modifications.
