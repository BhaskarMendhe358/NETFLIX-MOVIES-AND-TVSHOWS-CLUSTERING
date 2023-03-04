# NETFLIX-MOVIES-AND-TVSHOWS-CLUSTERING
Unsupervised Machine Learning NETFLIX-MOVIES-AND-TVSHOWS-CLUSTERING capstone project in which we had to cluster the content such that the show similar to each other and shows which are different are dissimilar to each other.


# Introduction : 
Netflix, headquartered in California, is a popular subscription streaming service and production firm. According to Statista, Netflix had approximately 220.67 million paid subscribers worldwide as of the second quarter of 2022. It is crucial that they effectively cluster the shows that are hosted on their platform in order to enhance the user experience for its subscribers. We will be able to understand the shows that are similar to and different from one another by creating clusters, which may be leveraged to offer the consumers personalized show suggestions depending on their preferences. The goal of this project is to classify/group the Netflix shows into certain clusters such that the shows within a cluster are similar to each other and the shows in different clusters are dissimilar to each other.



# EDA Summary

We found that movie content was present with most number than that of the TV-Shows.

Maximum rating that had most number of counts were TV-MA means the audience which was most engaged was Adults.

We also specified particular content rating with particular age and thus created new feature called age_category and we found Adults-3617,Teens -2314, Pre-Teens-1327, Kids-512.

We got Documentaries, Stand-up comedy, Darams & international TV are most watched genres in content type movies.

In TV-Shows we got Kids TV, International TV-Shows and TV dramas to be the most watched genres.

From Year_added we came to know that most of the movies were added in 2019 and most of the TV Shows were added in 2020.

From Month_added we came to know most of the content was added in start and end of the year must be at the time of Festival like Diwali, Christmas and New Year.

From day added we came to know that most of the content was added at the start of the month.

We came to know that the United States, India and United Kingdom are topmost countries in top 10 with maximum number of contents.

We came to know that all the countries except Japan and South Korea has maximum number of movies where United States and India tops the list.

We came to know that the most top most directors are from United States. It feels good when we see some Indian directors name among the Top 50 directors list around the world and they are S.S Rajamouli, Ram Gopal Verma, Suraj Barjatya and we hope in the future this names would be in the top.

It feels great to know that top most actors are from India and they are Anupam Kher, Om Puri, Shahrukh Khan.

Most of the words that were more often mentioned in title were love, christmas, man, story, world. We can say that movies are released during the time of Christmas and New Year i.e at the time of festivals.
We came to know that most words in description which are most often mentioned are family, new, life, find, freind.

We came to know that duration for most of the movies lasted for the 90-120 minutes.

Most of the TV-Show contents had 1 - 2 seasons and we came to know that contents with more than 6 seasons are rare.

We came to know that Netflix has been adding many International Tv Shows, Tv Dramas, Tv Comedy Shows and many more tv shows in the recent years compared to movies. From this observation, we can say that Netflix might be shifting slowly towards Tv Shows but not increasingly.

In India the count of TV-Shows was very less as Indian cinemas focuses on the movie content. In United States and United Kingdom the count of movies was maximum also they are focusing on TV-Show on large scale now a days.

We came to know that the maximum number of movies and tv-shows were added in 2019(movies = 1497, TV-Shows = 656) and 2020(movies = 1312, TV-Shows = 697) and from 2021 it gradually decreased.

The addition of the contents has gradually decreased from 2021 by maximum counts this must be due to the covid situations at the start of 2020. Now, the cinemas are coming in routine slowly and great movies are being added since 2021.

we came to know that most of the movies were released in the year 2017 i.e. 742 followed by 734 in 2018 And most of the TV-Show were released in the year 2020 i.e 457 followed by 2019 414. The counts were descrete from 2008 - 2011 then from 2012 it started increasing gradually.





# Clustering Summary : 
1.Clusters were built on the attributes: Director, Cast, Country, Rating, Listed in (genres), Description

2.Steps involved in preprosessing:Tokenize the corpus, Remove non-ascii characters, Convert all words to lowercase, Remove punctuation marks, Replace all numbers with its respective textual representation, Stemming and Lemmatization

3.Text corpus was vectorized using TFIDF vectorizer, and 20000 attributes were generated.

4.More than 80% of the variance is explained just by 4000 components. Hence to handle the curse of dimensionality, only the top 4000 components were taken, which will still be able to capture more than 80% of variance in the data.


# Conclusion

It was interesting to find that majority of the content available on Netflix is Movies.

TV-MA tops the charts, indicating that mature content is more popular on Netflix. Founded that Adults are more engaged over Netflix.

We got Documentaries, Stand-up comedy, Darams & international TV are most watched genres in content type movies.

In TV-Shows we got Kids TV, International TV-Shows and TV dramas to be the most watched genres

Most of these contents are released either in the year ending or the beginning. Most of the contents were added at the month end.

United States and India are among the top 5 countries that produce all of the available content on the platform.*

We found that 5 of the actors among the top ten actors with maximum content are from India.

From title we got most often used words such as Christmas, love, Man we can say that some of the particular content were targeted to release on Christmas day, New Year or other festivals.

We found K=4 as an optimal value for clusters in K-Means by elbow and sillhouette and From Agglomerative clustering we got 3 clusters using which we grouped our data into 3 distinct clusters.

Using the given data a simple recommender system was created using cosine similarity and recommendations for Movies and Tv Shows were obtained.




