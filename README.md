# AV-Jantahack-Recommendation-system
Approach to "Analytics Vidhya Janatahack: Recommendation system"

Hosted at: https://datahack.analyticsvidhya.com/contest/janatahack-recommendation-systems/#ProblemStatement

Rank: 52 from 12,064 registered participant.

Solution available in jupyter notebook form.

## Problem Statement:

Your client is a fast-growing mobile platform, for hosting coding challenges. They have a unique business model, where they crowdsource problems from various creators(authors). These authors create the problem and release it on the client's platform. The users then select the challenges they want to solve. The authors make money based on the level of difficulty of their problems and how many users take up their challenge.

The client, on the other hand makes money when the users can find challenges of their interest and continue to stay on the platform. Till date, the client has relied on its domain expertise, user interface and experience with user behaviour to suggest the problems a user might be interested in. You have now been appointed as the data scientist who needs to come up with the algorithm to keep the users engaged on the platform.

The client has provided you with history of last 10 challenges the user has solved, and you need to predict which might be the next 3 challenges the user might be interested to solve. Apply your data science skills to help the client make a big mark in their user engagements/revenue.

## Data Description

There are three files:

train.csv: It contains the set of 13 challenges that were attempted by the same user in a sequence. <br />
challenge_data.csv: Contains attributes related to each challenge <br />
test.csv: Contains the first 10 challenges solved by a new user set (not in train) in the test set. We need to predict <br />

##Solution
We used CPT(Compact Prediction Tree) Machine Learning Model to acheive this task.
Best result with below combination-
        k = 5, n=3 
        where,
        k is the number of last elements that will be used to find similar sequences and,
        n is the number of predictions required.
