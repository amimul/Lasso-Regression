# Lasso-Regression
Predicting goodness points of a wine given its reviews.

Implemented Coordinate Descent Algorithm along with Lasso Regression for predicting the goodness points of a wine.

The data was scraped from WineEnthusiast during the week of June 15th, 2017 and can be found on the analytics website Kaggle `https://www.kaggle.com/zynicide/wine-reviews`. This dataset provides a variety of features, the points, description (review), variety, country, province etc. For this project we used the points and description features. Points are ratings within range 1-100. However, the dataset contains description for wines rated in range 80-100. Feature vectors are already extracted for each review.

File | Description
---- | -----------
trainData.txt | **Training data matrix for predicting number of stars**
trainLabels.txt | **Training labels, list of the number of stars for each review**
valData.txt | **Validation data**
valLabels.txt | **Validation labels**
testData.txt | **Test data**
featureTypes.txt | **List of features used**

The data matrices are stored in Matrix Market Format, a format for sparse matrices. Each line is is a tuple of three elements for instance ID, feature ID, and feature value. Meta information for each feature is provided in `featureTypes.txt`. The features are strings of one, two, or three words (n-grams). The feature values correspond roughly to how often each word appears in the review. All rows have also been normalized.

Link for the Kaggle Competition
`https://www.kaggle.com/c/hw1-wine-goodness-cse512-spr18/leaderboard`
