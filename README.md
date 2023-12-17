Put your story line here and add your plot.html in /assets/plots/

Causal Analysis of Gender vs Rating

What makes people tick?

In this section of the study, we are trying to find what influences the ratings that people give for a movie. Since the ultimate goal of this study is to show the role that each gender has in the cinema, after this section, we will try to give a conclusive on in the question “Is the gender affecting the ratings that people give to movies in IMBD?” To do that, first we had to find a way to quantify the aspect of gender in a movie. To do that, we used the fraction of the female actors in the cast of the movie, i.e. how many of the actors are female in the movie in respect to the whole cast of the movie. Moreover, for a conclusive result, we needed to check the other movie characteristics that affect the ratings that people give, like the movie runtime, genre and more.

What do people vote?

Before diving deep into what influences the ratings, lets see first what people vote in general and how it changed across the years. This can give us some perspective on all the exciting cases that follow. Clearly visualized on the graph that follows, is that most of the votes are between 5-7 rating, showing that people tend to give a rating above average, or thinking differently, the average for a movie is a rating of 6.5.
But was that always the case? Let’s see is the average rating for the movies made each year changes along the years. We can distinguish two parts of the changes in rating. The first part show that in the start of the 20th century, up until around 1928, the average rating of the movies was increasing. The Pearson and Spearman correlations that give a p-value <0.05 reinforce this conclusion. However, the high 95% Confidence intervals suggest that the data are not that reliable. Then after 1928, the ratings start to decline as the years go by with negative significant correlation, with the data being more reliable.  
Now that we saw an overview of the ratings, let’s see some other parameters.

Runtime

Let’s continue down the list of questions. Do people generally prefer movies that run for a long time or do they prefer short movies, or are they indifferent to the duration of the movie?  Well, you can always find the answer here! For the most reliable data, for movies from around 60 to 200 minutes of runtime there can be seen a slight but statistically significant increase in the rating as the runtime goes up. It seems either that people like longer movies or if a movie is longer it is most likely to be better! 

Average age of the cast

Let’s now look at something else, the average age of the cast. Do people give higher ratings to movies that employ and cast older people? Or a younger, more vibrant and livelier cast is the way to go in order to get the people to give a good vote? With one quick look it seems that it does not actually matter. Both the Pearson and Spearman correlation statistics give a p-value around 0.5 which can help us reject the null hypothesis that the average age of the cast of the movie and the rating it gets are correlated. 

Genres, Languages and Country

Let’s continue to some distributions. Below we can see the distributions of the ratings for each genre and for languages and countries of the movies (we show countries and languages that more than 50 movies were made in each country and language). If there is a lot of variation between the distributions of the different categories for all these three variables, we can assume naively that there is some influence of the variable to the average rating. We can see that there is some variation of the average of the ratings, between 6 to 8, for the genres, 6 to 7.5 for languages and 6 to 6.7 for the countries. Therefore, we naively say that the genre and the language of the movie can influence the rating of the movie. 

Gender

Finally, it is time to address the elephant in the room, does gender play a role in the ratings that people give to the movies. As mentioned above, we are using the fraction of female actors in the movie. The naïve analysis shows that that there is a small but significant negative correlation between the female fraction of actors in the movie and the average rating. We can also see again that the female fraction of actors is generally below 0.35. This could be for a lot of reasons, for example people might like genres or that are best suited for male actors, or these genres are more carefully made. 

Is this really the case? 

Until now, we were looking at these cases naively and saw that many confounders can affect the average rating of a movie. To make sure that the fraction of female actors affects the average rating, we need to isolate its effect, that is we are going to perform a causal analysis. To do that we use a treatment and a control group. The treatment group is defined as the movies that have more female than male actors in their cast, whereas the control group is the opposite. So, we used propensity score matching for the above confounders that showed some correlation with the average rating. 
After matching we can see that the distribution of the average rating between the two groups is very similar, with the treatment group (more females than males in a movie) having a bit more probability to have around 4.5-7 and the control group a bit more probability above 7. The correlation statistics show a in the end that the fraction of female actors in a movie have little to no correlation to the average rating.

