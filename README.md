# song_popularity_prediction
Predicting song popularity on Spotify using a neural network involves leveraging various features of songs to train a model that can accurately forecast how popular a song might become
In the dataset, rows with null values are removed.
Important features used to predict song popularity were divided into two categories: numerical and categorical columns.
Numerical features are 'danceability', 'energy', 'key', 'loudness', 'mode','speechiness', 'acousticness', 'instrumentalness','liveness', 'valence', 'tempo', 'duration_ms'
Categorical feature was 'playlist_genre'.
Data was divided into training and validation data using GroupShuffleShift, to ensure all of an artist's songs in one
split or the other.
Data was preprocessed using OneHotEncoder and StandardScaler.
Neural network consisting of 5 layers was built and 'relu' was used as activation function. Batch Normalization and Dropout techniques were used to prevent overfitting and early_stop as callback for early_stopping.
Validation loss came about to be 0.195
