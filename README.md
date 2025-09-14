SongSphere is a Personalised Music Recommendation System that implements both Content-Based Filtering and Collaborative Filtering to recommend songs.

Recommender systems are widely used in industries such as music, movies, and e-commerce to personalize user experience. This project explores two main approaches:

1] Content-Based Filtering → Recommends songs based on similarity of features (e.g., lyrics, keywords). The recommendations done using content-based recommenders, can be seen as a user-specific classification problem. This classifier learns the user's likes and dislikes from the features of the song.

In a few words, the idea behind is to extract meaningful keywords present in a song description a user likes, search for the keywords in other song descriptions to estimate similarities among them, and based on that, recommend those songs to the user.

2] Collaborative Filtering → Recommends songs based on user-item interactions and preferences of similar users.
Collaborative-based filters predict what a user like based on what other users, that are similar to that particular user, have liked.

Datasets we have used -

Content-Based Dataset:

- Name: songdata.csv

- Size: 57,650 songs in English

- Source: Kaggle dataset (LyricsFreak scraped)

Collaborative Dataset:

- Name: songs.csv

- Size: Subset from Million Song Dataset

- Source: Million Song Dataset

How It Works

1️⃣ Content-Based Recommender :

- Extracts keywords from lyrics.
- Computes similarity scores between songs.
- Recommends songs with the most similar lyrics to those a user already likes. 
- It is Fast, interpretable, adapts well to new songs.
- Refer to - (content_based_music_recommender )
  
2️⃣ Collaborative Filtering Recommender :

- Uses a user-item rating matrix.

- Predicts if a user will like a song based on preferences of similar users.

- Two approaches: a] User-User Filtering → Find similar users and recommend what they like.
                  b] Item-Item Filtering → Find similar songs based on ratings.
- Refer to - 1) CF_knn_music_recommender and
             2) CF_matrix_fact_music_recommender



