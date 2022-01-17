# Week_3
## Overview of Election Audit
The purpose of this audit was to provide a user friendly breakdown of the csv election data. We were able to get a clear picture of many things including how many candidates were up for election, how many votes each candidate got, how many counties contributed to the election, and which county had the most votes submitted.

## Election-Audit Results
### How many votes were cast in this congressional election?
There were 369,711 ballots cast.
### Provide a breakdown of the number of votes and the percentage of total votes for each county in the precinct.
| County  | Total Votes | Percent of Total |
| :-------------: |:-------------:| :-----:|
| Jefferson  | 38,855 | 10.5% |
| Denver   | 306,055  | 82.8% |
| Arapahoe | 24,801 | 6.7% |

Percent of Total achieved by code `countyPercent = float(countyVoteCount)/float(total_votes) *100`
### Which county had the largest number of votes?
The largest number of votes came out of Denver county. This was represented by _winningCounty_ variable
### Provide a breakdown of the number of votes and the percentage of the total votes each candidate received.
| Candidate  | Total Votes | Percent of Total |
| :-------------: |:-------------:| :-----:|
| Charles Casper Stockham  | 85,213 | 23.0% |
| Diana DeGette   | 272,892  | 73.8% |
| Raymon Anthony Doane | 11,606 | 3.1% |

Percent of Total achieved by code `vote_percentage = float(votes) / float(total_votes) * 100`
### Which candidate won the election, what was their vote count, and what was their percentage of the total votes?
The winning candidate was Diana DeGette with 272,892 votes. She had 73.8% of the total votes

## Election-Audit Summary
Given time this code could be adapted to many other election audit situations. Below are 2 way this code could be edited to use for future elections.
1. By adapting where the file is read from you could choose a new csv file to pull information from. We would replace the election_results.csv to another file name. We would also adjust the pathing to either place this new csv file into the resources folder or change the "Resources" section to reflect the new folder path. `file_to_load = os.path.join("Resources", "election_results.csv")` At the same time, we would adjust the output as well. `file_to_save = os.path.join("analysis", "election_analysis.txt")` In the same manner we would make a new txt file and adjust it pathing accordingly
2. Depending on data presented we may need to adjust our code. If the csv file is separated by something other than a comma such as a colon we should adjust the code as follows: `reader = csv.reader(election_data, delimiter=":")` Additionally, if the file has the needed information in different "columns" within the csv file we may need to edit the code such that `candidate_name = row[x]` where x is the correct array number corresponding to the file.
