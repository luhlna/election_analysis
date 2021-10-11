# Election_Analysis
Use the power of  Python to automate the vote - counting process for a local election.

## Proyect Overview
Tom is a Board of Election employee, who has asked our help to audit the results for the US’ election of Congressional precinct in colorado. They are looking to automate the process using Python of reporting the total number of votes cast, the total number for each candidate, the percentage votes for each candidate, ande the winner of the election based on the popular vote.

## Resources
- Data Source: election_results.csv
- Software: Python 3.7.6, Visual Studio Code  1.60.2

## Summary
From a data sample of 369,711 registered votes we found there were 3 candidates:
- Charles Casper Stockham
- Diana DeGette
- Raymon Anthony Doane

And when running some analysis we determine the results were:
- Charles Casper Stockham recivied 23.0% of the vote and 85,213 number of votes.
- Diana DeGette recived 73.8% of the vote and 272,892 number of votes.
- Raymon Anthony Doane recieved 3.1% of the vote and 11,606 number of votes.

Therefore we could determine the winner:
- **Diana DeGette**, who recieved 73.8% of the vote and 272,892 number of votes.

## Challenge Overview
Thanks to the oustanding results of the election audit, Tom asked some additional data to complete the previous audit:
- The voter turnout for each county
- The percentage of votes from each county out of the total count
- The county with the highest turnout

## Challenge Summary
We worked again with the same set of data to gather now information of each of the three counties:
- Jefferson
- Denver
- Arapahoe

From which we determined that:
- Jefferson County represents 10.5% of the vote with 38,855 number of voters.
- Denver County represents 82.8% of the vote with 306,055 number of voters.
- Arapahoe County represents 6.7% of the vote with 24,801 of voters.

Where the largest County turnout was: **Denver**

Finally we succesfully delivered the analysis required for the audit project, nevertheless this code can be adjusted and replicated for other precincts or elections. e.g.

Selecting the correct file paths
```
# Add a variable to load a file from a path.
file_to_load = os.path.join("Resources", "election_results.csv")
# Create a filename variable to a direct or indirect path to the file.
file_to_save = os.path.join("analysis", "election_analysis.txt")
```
It's key to any further analysis to select the correct path for the source elements to get proper communication with the code.

Review the data formath
```
# Read the header
    header = next(reader)
    print(headers)
```
For compatibility purposes between of this code and the new sets of data is important to ensure the CSV file has the same structure; so all the variables stated can run properly.
![data-3-3-1-first-10-rows](https://user-images.githubusercontent.com/90527212/136732817-088d0be1-b570-4a7b-85c1-662e2cab9921.png)
