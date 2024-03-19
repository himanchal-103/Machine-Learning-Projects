# Youtube Adview Predictions

This project aims to predict the number of adviews a YouTube video will receive based on various factors such as video duration, category, upload date, etc. Adviews are crucial for content creators and advertisers to understand the popularity and reach of their videos.

# Dataset details
The file train.csv contains metrics and other details of about 15000 YouTube videos. The metrics include the number of views, likes, dislikes, comments, published date, duration, and category are also included. The file also contains the number of adviews which is our target variable for the prediction

Attribute Information
1. 'vidid': Unique Identification ID for each video
2. 'adview': The number of adviews for each video
3. 'views': The number of unique views for each video
4. 'likes': The number of likes for each video
5. 'dislikes': The number of likes for each video
6. 'comment': The number of unique comments for each video
7. 'published': The data of uploading the video
8. 'duration': The duration of the video (in min. and seconds)
9. 'category': Category niche of each of the video

# Objective
To build a machine learning regression to predict youtube adview count based on other youtube metrics.

# Steps and Tasks
1. Import the datasets and libraries, check shape and datatype.
2. Visualise the dataset using heat maps and plots. You can study data distributions for each attribute as well.
3. Clean the dataset by removing missing values and other things.
4. Transform attributes into numerical values and other necessary transformations
5. Normalise your data and split the data into training, validation, and test sets in the appropriate ratio.
6. Use Linear Regression, SVM, Decision Tree, and Random Forest algorithm.
7. Pick the best model based on error as well as generalization.
8. Save your model and predict on the test set.
