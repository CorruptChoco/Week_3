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
Given time this code could be adapted to any election audit situation. Below are 2 way this code could be editted to use for future elections.
1. 
2. 
