# Election Audit
Election Analysis Using Python

## Overview 
This project focuses on the application of Python code to analyze a .CSV file with congressional election results. The source file contains 369,711 votes for one of three candidates cast throughout three counties. This report will describe the outcomes of this election audit, and explains how the code written for this analysis can be generalized for use with other similar data files.

## Election-Audit Results
- Because each row in the data sheet represents one vote, the total amount of votes cast was determined by creating a loop that runs through tha data file and adds 1 to the total_votes counter for each row in the sheet, disregarding the first row that contains headers:

![image](https://user-images.githubusercontent.com/93882635/145748940-ac47bbd6-972b-436e-9f01-7f34e1d123dd.png)

This results in a total of 369,711 votes cast.

- To break down the total number of votes by county, a list of counties was compiled using an If-statement. The code adds counties to the list, and starts a counter for each of them. The percentage of total votes for each county in the precinct was determined by dividing the number of votes cast per county by the number of total votes and multiplying the result by 100.

![image](https://user-images.githubusercontent.com/93882635/145749794-c5bee6bf-c3f8-41d3-ac8c-9648da7b60c3.png)

The resulting analysis shows that Denver County had the largest number of votes: 306,055 (82.8% of total votes)

- A list of candidates was compiled in a way similar to the list of counties. A counter was started for each of the candidates, with one vote being added for every row that contained their name. In this way, the code was able to declare amount of votes received by each candidate, showing that Charles Casper Stockham reiceived 23.0% of the votes (85,213 votes), Diana DeGette received 73.8% of votes (272,892 votes), and Raymon Anthony Doane received a mere 3.1% of votes (11,606 votes).

- This analysis shows that Diana DeGette is the undisputed winner of this election with a total of 272,892 votes, a whopping 73,8% of all votes cast.

## Election-Audit Summary
The usefulness of the code used for this analysis is not limited to this particular example. It is highly adaptable and can handle any list of election results.
- The code is capable of compiling a list of candidates. If more than three candidates were present, the list would be updated with any additional candidates, and output the result for each of them.
- In a similar way, the code is able to add any additional counties to the list. With minor modifications, the code is able to handle elections on different levels too: Counties can be substituted with County districts during a council member election, or even entire States during a presidential election.
