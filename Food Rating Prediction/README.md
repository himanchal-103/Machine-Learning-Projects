# FOOD RECIPE RATING PREDICTION

## Aim
This project aims to develop machine-learning pipelines for predicting the ratings of food recipes by leveraging both numerical and textual data.

## Dataset
The dataset is composed of the following files:
1. train.csv: The training set contains 13636 records, which includes the target variable 'rating' and accompanying feature attributes.
2. test.csv: The test set includes 4568 records and contains similar feature attributes but without the target variable 'rating', as it is the variable to be predicted.

Columns Description: 
1. ID
2. RecipeNumber: Placement of the recipe on the top 100 recipes list
3. RecipeCode: Unique ID of the recipe used by the site
4. RecipeName: Name of the recipe the comment was posted on
5. CommentID: Unique ID of the comment
6. UserID: Unique ID of the user who left the comment
7. UserName: Name of the user
8. UserReputation: Internal score of the site, roughly quantifying the past behavior of the user
9. CreationTimestamp: The time at which the comment was posted as a Unix timestamp
10. ReplyCount: Number of replies to the comment
11. ThumbsUpCount: Number of up-votes the comment has received
12. ThumbsDownCount: Number of down-votes the comment has received
13. Rating: The score on a 1 to 5 scale that the user gave to the recipe. A score of 0 means that no score was given (Target Variable)
14. BestScore: Score of the comment, likely used by the site to help determine the order comments appear in
15. Recipe_Review: The text content of the comment


## Model

1. The first pipeline utilizes a TFIDF vectorizer to convert text data into numerical features, followed by a logistic regression model for prediction. 
2. The second pipeline employs a CountVectorizer for text transformation and a Random Forest classifier for prediction.

Both pipelines are evaluated to determine their performance and effectiveness in rating prediction.

