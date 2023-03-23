# 2022 GWU-Datathon 
## Research question: 
What tweet topics can bet most retweets?
## Dataset information:
The dataset is pulled from Twitter's rest API and provided by Finsburg Glover Hering. Each row of data collects features about a single tweet such as user data (like name, screen name, follower count, verified, etc); tweet information (like tweet text, created at, etc.); engagement data (like retweet count, favorite count, reply count, etc); etc. This is a high dimensional dataset and will require manual pre-processing to subset relevant predictor features.

My response variable is "retweet_counts", which I categorized it into three levels: low(5 or less), medium(6-99) and high(100 or more).
## Guideline:
Data preprocessing - EDA - Hypothesis testing(optional) - Model selection and validation - Results interpretation - Recommendations.
## A quick go-through what I did:
I took a random subsample of 10K datapoints just for less model running time.

I did NLP for "tweet_text". Used Latent Dirichlet Allocation(LDA) model to generate six topics based on tokens from "tweet_text". Then I used multinomial logistic regression model to predict what are the best topics to get most retweets.

My intention is to get more familiar with NLP techniques in this Datathon rather than doing some findings. So there may be some errors along the project. But still, it's a beginner-friendly learning project.
