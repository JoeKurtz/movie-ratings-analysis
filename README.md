# Movie Ratings Analysis (Group Project)
Analyzing the Change in Movie Ratings within a Movie Series

## Idea Formation

After being handed this assignment with the IMDB dataframe, we wondered to ourselves what exactly we were going to anaylyze. Each memeber of our group are self-identified movie fanatics, where one of our favorite hobbies is to sit back and watch a movie with some friends.

After discovering that each of us love to watch movies, we asked each other what movie was our individual favorites. Needless to say, this led to a ton of disagreement. A big factor on judging whose movie was better was rating the consistency of the movie - that is, how well did the sequel of the movie perform in our minds? Did it live up to the hype of the first one? Was the sequel a flop?

While some of our favorite movies were solos movies (i.e. there was no sequel), most of our favorites were part of a series. To add to this, Hiram, a key member of team JHI, argued that sequels to a movie NEVER (in caps on purpose - he assetered this rather emphatically) live up to the first movie. I [Joe] had to argue to back on this - after all, the Harry Potter movies seemingly got better over time!

This led us to our question, our topic of interest, if you will, one that asked:

## _**How do Movie Ratings Fluctuate Throughout a Movie Series?**_
We needed to put this argument to rest. Particularly, we wanted to know if in fact sequels and subsequent movies as part of a series actually performed worse, or if this was just misconception.

Some Famous Movie Series' We Looked At:

The Godfather
The Matrix
The Maze Runner
Men in Black
Lord of the Rings
Spider-Man
Back to the Future

Before I get into the finding, I believe it is impertive to list out some limitations we faced:

## Limitations
First off, and most obvious, our sample of movies isn't exactly a random sample; Each movie series are among the more popular movie series' and hence the statistics would be a bit skewed. While we know this is true, we believe the general idea of our analysis still has validity, and the coding aspect is definitely strong.
Second off, for a real statistical sample, our data would have to be normal to perform these calculations. We acknowledge this, and also would like to note that a linear regression would be more telling too in analyzing the trends.
Third off, and lastly, our sample size is too small for a real analysis. However, like aforementioned, the coding aspect of our analysis is strong, even if real implications cannot be assumed.

## Analysis Process
The Process of our analysis was as follows:

IMDB:

Use SQL JOINs and different queries to collect the desired movies for analysis, seperated by the Movie Title and its Average Rating
Each Movie was then assigned to a variable for plotting purposes
Following the SQL queries for selecting our movies, we then plotted each movie with the x-axis being the movie number (plotted by index) and the y-axis being its average rating
Looking at the data and the plots, we then analyzed the general trend of the movie ratings
We then compiled each movie and its ratings into a dataframe, with the columns being the individual movie series and the rows being the movies ratings plotted by index
With this dataframe, we took the mean of each index (i.e. the mean of all ratings of the first movies of the series, the seconnd movies,...) and plotted the results on a graph
Looking at the data and the plots, we then analyzed the general trend of the movie ratings
Rotten Tomato:

Use Pandas filtering to collect the desired movies for analysis, seperated by the Movie Title and its Average Rating
We then plotted each movie with the x-axis being the movie number (plotted by index) and the y-axis being its Tomoto-Meter Score
Looking at the data and the plots, we then analyzed the general trend of the movie ratings
We then compiled each movie and its ratings into a dataframe, with the columns being the individual movie series and the rows being the movies tomato score plotted by index
With this dataframe, we took the mean of each index (i.e. the mean of all scores of the first movies of the series, the seconnd movies,...) and plotted the results on a graph
Looking at the data and the plots, we then analyzed the general trend of the movie ratings
Now, into the results of our analysis:

## Findings
Looking at the IMDB Data first, we see the trend of movie ratings decreasing over time. Generally, for our sampled movie series, the first movie in the series was the highest rated movie in the series. Gradually, as subsequent movies within the same movie series were produced, the ratings decreased, never to recover to the first movie's ratings.

This trend holds true for 6/7 movies analyzed. The only outlier in this select sample was Lord of the Rings, where the second movie was the highest rated, while all three were both closely and highly rated.

Putting the analysis' limitations to the side, we were able to accept the null hypothesis that the ratings decrease as subsequent movies are produced.



This observation is confirmed by the Rotten Tomato data. Similar to the IMDB ratings, as subsequent movies within the same movie series were produced, the ratings decreased, never to recover to the first movie's ratings.

While using IMDB's ratings 6/7 movies confirm that finding, simply looking at Rotten Tomato scores, only 4/7 movies follow that trend, while Spider-Man 2 rated higher than Spider-Man, and The Godfather II rated equally to The Godfather.

Putting the analysis' limitations to the side, we could not accept (or reject)the null hypothesis that the ratings decrease as subsequent movies are produced from the Rotten Tomato data as the data is inconclusive.

Obviously, however, from a statistics standpoint, the data collected is not substantial enough to either accept or reject our null hypothesis that movie ratings decrease through out a movie series
