TMDB 5000 Movie Recommendation System:
Clustering problem [Unsupervised Learning]

Notebook Link:
https://drive.google.com/file/d/1WsAu48DX_gu3skktqtDu1EIp50SGu8t4/view?usp=sharing

Dataset:
https://www.kaggle.com/tmdb/tmdb-movie-metadata

EDA:
I have used matplotlib.pyplot library.Matplotlib is a comprehensive library for creating static, animated, and interactive visualizations in Python.matplotlib.pyplot is a state-based interface to matplotlib mainly intended for interactive plots.

The barh() function within this library is used to draw a horizontal bar plot of 10 most popular movies.The bars are positioned at y with center alignment.

Models:
1.Content Based Filtering- 
It suggests similar items based on a particular item. This system uses item metadata, such as genre, director, description, actors, etc. for movies, to make these recommendations. The general idea behind these recommender systems is that if a person liked a particular item, he or she will also like an item that is similar to it.In this recommender system the content of the movie (overview, cast, crew, keyword, tagline etc) is used to find its similarity with other movies. Then the movies that are most likely to be similar are paired (i.e. clustered) and then recommended.

2.Demographic Filtering- 
It offers generalized recommendations to every user, based on movie popularity and/or genre. The System recommends the same movies to users with similar demographic features. The basic idea behind this system is that movies that are more popular and critically acclaimed will have a higher probability of being liked by the average audience.

Results-

1.Content Based Filtering- 

Recommendations for 'Avatar' movie-

3604                       Apollo 18
2130                    The American
634                       The Matrix
1341                Obitaemyy Ostrov
529                 Tears of the Sun
1610                           Hanna
311     The Adventures of Pluto Nash
847                         Semi-Pro
775                        Supernova
2628             Blood and Chocolate

2.Demographic Filtering- 
The 10 most popular movies are-
1.Minions
2.Interstellar
3.Deadpool
4.Guardians of the Galaxy
5.Mad Max: Fury Road
6.Jurassic World
7.Pirates of The Caribbean:The Curse of the Black Pearl
8.Dawn of the Planet of the Apes
9.The Hunger Games: Mokingjay -Part 1
10.Big Hero 6


