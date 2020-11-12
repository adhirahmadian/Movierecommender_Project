# Movierecommender_Project

# Overview
I used content-based recommender systems to see movie recommendations based on the similarity between my preferences.

# Code Resources

Python Version: 3

Packages: pandas, numpy, matplotlib, seaborn.

The dataset is obtained from https://grouplens.org/datasets/movielens/ with small size version 
(100,000 ratings and 3,600 tag applications applied to 9,000 movies by 600 users(Last updated 9/2018))

# EDA

I count the most reviewed movie in the dataset.

Movie Title | Total Review
------------ | -------------
Forrest Gump (1994)  | 329
Shawshank Redemption, The (1994) | 317
Pulp Fiction (1994) | 307
Silence of the Lambs, The (1991) | 279
Matrix, The (1999) | 278
... | ...

I make table of movie title and rating based on most total review in the dataset.

Movie Title | Rating | Total Review
------------ | ------------- | -------------
Forrest Gump (1994)	| 4.164134 |	329
Shawshank Redemption, The (1994) |	4.429022 |	317
Pulp Fiction (1994) |	4.197068 |	307
Silence of the Lambs, The (1991) |	4.161290 |	279
Matrix, The (1999) |	4.192446 |	278
Star Wars: Episode IV - A New Hope (1977) |	4.231076 |	251
Jurassic Park (1993) |	3.750000 | 238
Braveheart (1995) |	4.031646 |	237
Terminator 2: Judgment Day (1991) |	3.970982 |	224
Schindler's List (1993) |	4.225000 | 220
... | ... | ...


# Recommendation of Movie

For example, I want to watch another movie like starwars, so here it is top 5 recommendation from the algorithm.

Movie Title | Correlation | Total Rating
------------ | ------------- | -------------
Star Wars: Episode IV - A New Hope (1977) |	1.000000 |	251
Star Wars: Episode V - The Empire Strikes Back (1980) |	0.777970 |	211
Star Wars: Episode VI - Return of the Jedi (1983) |	0.734230 |	196
Fugitive, The (1993) |	0.482078 |	190
Indiana Jones and the Last Crusade (1989) |	0.410916 |	140

The value of Correlation represent of a-movie-that-is-look-like, the higher the value (max = 1) the more like the movie.

another example i want to watch movie-like Jurassic Park, so here it is top 5 recommendation from the algorithm.

Movie Title | Correlation | Total Rating
------------ | ------------- | -------------
Jurassic Park (1993) |	1.000000 |	238
Outbreak (1995) |	0.533780 |	101
Ghostbusters (a.k.a. Ghost Busters) | (1984) |	0.522286	120
Fugitive, The (1993) |	0.460603 |	190
Indiana Jones and the Temple of Doom (1984) |	0.456533 |	108

> for the complete explaination, please refer to .ipynb file
