# Amazon_Fine_Food_Reviews_Analysis

Amazon.com, Inc., is an American multinational technology company based in Seattle, Washington. Amazon focuses on e-commerce, cloud computing, digital streaming, and artificial intelligence. As they are strong in e-commerce platforms their review system can be abused by sellers or customers writing fake reviews in exchange for incentives. It is expensive to check each and every review manually and label its sentiment. So a better way is to rely on machine learning/deep learning models for that. In this case study, we will focus on the fine food review data set on amazon which is available on Kaggle.

# About Data set
The data set consists of reviews of fine foods from amazon over a period of more than 10 years, including 568,454 reviews till October 2012. Reviews include rating, product and user information, and a plain text review. It also includes reviews from all other Amazon categories.
We have the following columns:
Product Id: Unique identifier for the product
User Id: unique identifier for the user
Profile Name: Profile name of the user
Helpfulness Numerator: Number of users who found the review helpful
Helpfulness Denominator: Number of users who indicated whether they found the review helpful or not
Score: Rating between 1 and 5
Time: Timestamp
Summary: Summary of the review
Text: Review

# Basic Text Preprocessing
As a step of basic data cleaning, we first checked for any missing values. Fortunately, we don’t have any missing values. Next, we will check for duplicate entries. On analysis, we found that for different products the same review is given by the same user at the same time. Practically it doesn’t make sense. So we will keep only the first one and remove other duplicates.

# Preprocessing text data
Text data requires some preprocessing before we go on further with analysis and making the prediction model. Hence in the preprocessing phase, we do the following in the order below:-
Begin by removing the Html tags.
Remove any punctuation’s or a limited set of special characters like, or . or #,! etc.
Check if the word is made up of English letters and is not alpha-numeric
Convert the word to lowercase
Finally, remove Stopwords

# Converting Text to N dimensional vector
