# Election_Analysis

## Project Overview
A Colorado Board of Elections employee has given you the following tasks to complete the elcetion audit of a recent local congressional election.

1. Calculate the total number of votes cast.
To calculate the total number of votes, we established the rows to loop though, and created a "for loop" which went through every row in the provided data. For each row it added an additional vote to the total votes counts.

#(for row in reader:
        Add to the total vote count
        total_votes = total_votes + 1)

2.Get a complete list of candidates that recieved votes
To get the list of candidate names we set up a condition in the loop, whenever a candidate name was found that was not yet in out candidate names list yet, it gets added.

#(if candidate_name not in candidate_options:
       candidate_options.append(candidate_name))

3. Calculate the total number of votes each candidate recieved
To calculate the number of votes for each candidate, we first had to set their votes to zero. Then add to the loop that whenever it sees that the candidate was voted for, it will add a vote to their count.

#       (candidate_votes[candidate_name] = 0
#candidate_votes[candidate_name] += 1) 
4. Calculate the percentage of votes each candidate won.
To calculate the percentage of votes we collected the number of each candidate got then divided it by the total number of votes.

 #(votes = candidate_votes.get(candidate_name)
        vote_percentage = float(votes) / float(total_votes) * 100)

5. Determine the winner of the election based on popular vote.
We figured out the winner by comparing the votes they got to the total number. As well as doing that for the percentages as well

#(if (votes > winning_count) and (vote_percentage > winning_percentage):
            winning_count = votes
            winning_candidate = candidate_name
            winning_percentage = vote_percentage)

## Resources 
- Data Source: election_results.csv
- Software: Python 3.7.6, Visual Studio Code, 1.68.1

## Summary
The analysis of the elections show that:
- There were "x" votes cast in this election
- The candidates were:
  - Candidate 1
  - Candidate 2
  - Candidate 3
- The candidate results were.
  - Candidate 1 recieved "x%" of the votes and "y" number of votes
  - Candidate 2 recieved "x%" of the votes and "y" number of votes
  - Candidate 3 recieved "x%" of the votes and "y" number of votes
- The winnter of the election was:
  - Candidate (1, 2, or 3), who recieved "x%" of the vote and "y" number of votes
  
## Chalange Overview

## Challange Summry
