MUSIC

Introduction
Music is an implicit part of our life. It has the power to make or break a mood, inspire a change, or make you feel like the star of a music video. Music is a common language. It spreads across multiple cultures, societies and genres.
A study conducted in 2011 [1], showed that mood and performance directly correlate with music. Infact a viral trend started that used mario-kart theme song to help increase the speed of your work, while slow tunes help you focus longer. Multiple studies [2] conducted over the years, all point to a single conclusion "Music directly affects you".
So when you're studying for ML and need music to be creative or need music to finish the assignment fast, you need a perfect playlist. But creating a playlist can take a while. This is where music recommendation system can help. Spotify, a MRS giant, is known for its music recommendation. Spotify uses a host of algorithms to determine what kind of music an individual may like [3]. They use user activity and collaborative filtering to recommend songs.
But does this provide the best recommendations or just a set of songs you may or may not like? A study conducted in 2018[4] highlights some of the issues with this kind of recommendation systems. Another paper provides a critical analysis of MRS [5]. Once of the issues highlighted is situational recommendation.
Say you are listening to relaxational music while doing ML Assignment, this is a passive activity where music in your playlist auto plays songs in the background while you work. What if you don’t have a playlist or found one song that you like and forgot to add more to the queue. How should the next song be decided? Classic MRS finds any song that you may like and play it, this may or may not be a relaxational music but still may be a song that you enjoy. This random selection disturbs your mood and thereby affects your performance.

Problem Definition 

For the unsupervised learning part of this project, we want to explore  

(1) how to categorize every song into different clusters based on their characteristics (e.g.: danceability, loudness) and then  

(2) how to make music recommendations to users based on their preferences and our clustering results 

We are aware that data on the users’ side such as age, gender, liked songs, music listening behavior is often needed if we want to make music recommendations. However, this kind of data is not available using the Spotify API. To make our project easier, we could just let users enter 1 of their favorite songs and recommend top N songs that are the most similar to the ones they entered. 

For the supervised learning part, we could use regression to figure out how characteristics impact their popularity score and build a model to predict the popularity score. 

 
Methods 

For the unsupervised learning problem, we could leverage K-means and GMM (and hierarchical clustering if time permits) for clustering.  And then we could use Euclidean (or other) distance to decide which song(s) are nearest to users’ liked songs within the same cluster. Finally, we could select the top N nearest songs as recommendations. 

For the supervised learning problem, we could leverage linear regression, logistic regression and possibly random forest to model and predict the popularity. 


Potential results and Discussion 

Ideally, we’ll be able to cluster different songs into different categories, understand how popularity is decided and able to generate some songs based on users’ preferences. Metrics we’ll use to evaluate our results will include but not limit to completeness score (for clustering problem) and R^2, MSE (for the regression problems). 

 

Citations:  
https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0018861

https://www.heartmath.org/assets/uploads/2015/01/music-mood-effects.pdf

https://www.music-tomorrow.com/blog/how-spotify-recommendation-system-works-a-complete-guide-2022#:~:text=%22We%20can%20understand%20songs%20to,recommend%20song%20Z%20to%20them.

https://maroo.cs.umass.edu/getpdf.php?id=1289

https://orca.cardiff.ac.uk/id/eprint/145695/1/A%20Critical%20Analysis%20of%20Music%20Recommendation%20Systems%20and%20New%20Perspectives.pdf

Samoshyn,  Andrii. (2020). Dataset of songs in Spotify, Version 1. Retrieved on Oct 6, 2022, from https://www.kaggle.com/datasets/mrmorj/dataset-of-songs-in-spotify. 

Morris, M. (2021). Spotify Top 100 Songs of 2010-2019, Version 4. Retrieved on Oct 6, 2022, from https://www.kaggle.com/datasets/muhmores/spotify-top-100-songs-of-20152019. 


