
## Readme

* **Goals and Objectives**: 
    
    Hello everyone, in this notebook we are going to be exploring the our gathered data on behalf of Microsoft to gain insights about the movie industry. We are looking to find out if the two main methods of reporting on if a movie was successful (rating and profit margin) are actually indicative of a movie's success. Then using that information we will attempt to find some useful insights that we can apply to any future movie endeavor down the road.


* **Question 1**: Is Rating a good measure of success?
    1. First we joined the imdb_title_basics and the imdb_title_ratings dataframes together to view the movie title and rating information side by side using pandas. Then we dropped our null values and grouped the data by year and pulled the mean for each year in an attempt to view any trends about how ratings have changed over the years. 
    2. We did manage to discern that the average rating for movies has been going up year by year which shows that due to the modernization of platforms giving the average person the ability to review movies with much more ease then in the past, the average rating is increasing due to that. We chose to look at the average rating vs number of ratings becuase we know that the number of ratings is bound to go up based on modernization but the value of those ratings is paramount to us here. In the future we wonder if gathering data like in person interviews or looking through written reviews for certian keywords would be more benefical to finding useful information from the ratings.

* **Question 2**: What month of release has the best profit margins?
    1. First we used SQL to join the tables of tn_movie_budgets and imdb_title basics for the primary title info and budget and profit data. Then we created a profit and profit margin columns to better assess if a movie was successful financially vs a less indicative number like gross worldwide gross. Then we found the movies with the highest profit and highest profit margin across the industry. Then we used that data combined with the release_date data to gain insight into the month of release and how it impacted the movies profit margin. We converted the release date data into individual columns for year, day and month. We then were able to average the profit margins for each month.
    2. We discovered that June was the most profitable month of the year to release a movie on which can be done easily by a studio during the planning phase. We don't specifically know what drives this month to be more profitable then others, we have some assumptions like kids being out of school, but we would need to do some further research to be sure. 

* **Question 3**: What day of the week is best to release on for the highest profit margins?
    1. First we used our previous dataframe used in Question 2 and created a column that told us what day of the week the movie was released on. We then used the average of each day of the week's profit margin to discern which day of the week was the best to release a movie on.
    2. We found that Friday is by far the best day to release a movie on for the highest profit margins. We don't specifically know what drives this day to be more profitable then others, we have some assumptions, like it being the first day of the weekend and if people get to bed late they have the entire weekend to recover their sleep on, but we would need to do some further research to be sure. 

* **Future Research**: For future work we would like to look into the following areas.
    1.  The effect that a director's experience has on the profit margin of a movie.
    2. Also we'd like to look into the variances of genre, say for example between when specific genres are best to release for profit and when the market would be most crowded with a similar type of movie.
    3. We also would like to look into gathering different kinds of data (say data from in person interviews or written reviews of the movie) to gain more insights from how people feel about a movie itself.
    4. Lastly the subjective question of "What makes a movie successful?" would be interesting to explore. We obviously looked into profit here as a main indicator of success, but perhaps something like creating a movie that is unique for its genre would be considered "successful", or something like a movie about a good cause, or a movie covering controversial topics.
