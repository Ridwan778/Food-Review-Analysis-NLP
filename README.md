# Food Review Analysis using NLP

## The goal of this project was to explore how well the VADER module from the NLTK toolkit performs in identifying good and bad reviews.

## How to run:
1. Install Anaconda if already not installed. Visit this page for more information on how to do that - https://docs.anaconda.com/free/anaconda/install/windows.html
2. Open Jupiter Notebook from inside Anaconda and navigate to the project repository.
3. Open the food_review_sentiment_analysis.ipynb file to run the program.
   
## Construction:
1. We used NLTK libraries' pre-trained sentiment analyzer VADER to classify whether a review was positive or negative.
2. Then we compared this classified data with user ratings(1-5 stars) using a scatterplot to see how well the VADER model performs.
3. We also created word clouds with the most used words from both the best and worst reviews according to both user ratings and VADER for ease of visualization.

![5-star review words](https://github.com/Ridwan778/Product-Review-Analysis/assets/113521598/7c6d8d5c-1309-403e-b5a7-92ed4e602201)
![postive_sentiment_words](https://github.com/Ridwan778/Product-Review-Analysis/assets/113521598/248cba2e-77f7-42e7-b6ca-32cc96b40ade)

![1 and 2 star review words](https://github.com/Ridwan778/Product-Review-Analysis/assets/113521598/b3e12499-2d00-4f55-84b4-0578eee5ed00)
![negative_sentimeent_words](https://github.com/Ridwan778/Product-Review-Analysis/assets/113521598/c6ef0a74-1d0f-48e6-b189-7f1143d0f4e1)

![Scatterplot(VADER vs Ratings)](https://github.com/Ridwan778/Product-Review-Analysis/assets/113521598/c0f47a18-9ff1-4c96-9180-d28125fabedb)


## Observations:
1. Comparing the word clouds of 5-star reviews and positive sentiment reviews(according to VADER) we can see that both have very similar words but different frequencies. Both have positive adjectives such as great, best, nice, etc. So we can say VADER performed well here.

2. Similarly for 1&2 star reviews and negative sentiment reviews we observe negative adjectives such as awful, terrible, etc. in both their wordclouds.

3. But when we compare each reviews' compound scores we got from VADER model to their star ratings using a scatterplot we can notice that for lot of 5-star reviews the the sentiment intensity analyzer gives a very low compound score. At the same time for many 1 star reviews it gives the maximum compound score of 1.0.
  
5. Therefore, VADER model's sentimental analysis is not always pinpoint accurate, but it generally gets things right.
