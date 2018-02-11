## Music Recommender System using Apache Spark and Python

[1]: http://www-etud.iro.umontreal.ca/~bergstrj/audioscrobbler_data.html

Creating a recommender system that will recommend new musical artists to a user based on their listening history. Suggesting different songs or musical artists to a user is important
to many music streaming services, such as Pandora and Spotify. In addition, this type of recommender
system could also be used as a means of suggesting TV shows or movies to a user (e.g., Netflix).

## Techniques Used
1. Collaborative Filtering
2. Spark
3. Jupyter

## Datasets
Publicly available song data from audioscrobbler, which can be found [here][1]. However, we modified the original data files so that the code will run in a reasonable time on a single machine. The reduced data files have been suffixed with `_small.txt` and contains only the information relevant to the top 50 most prolific users (highest artist play counts).

Note that when plays are scribbled, the client application submits the name of the artist being played.
This name could be misspelled or nonstandard, and this may only be detected later. For example, "The
Smiths", "Smiths, The", and "the smiths" may appear as distinct artist IDs in the data set, even though
they clearly refer to the same artist. So, the data set includes artist_alias.txt, which maps artist
IDs that are known misspellings or variants to the canonical ID of that artist.
The artist_data.txt file then provides a map from the canonical artist ID to the name of the artist.

## How to run
1. Start jupyter using `jupyter notebook`.
2. Run all cells in `recommender.ipynb`.
