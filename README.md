# Project-1

# Objective
The purpose of the project was to use the Top 5 Spotify Songs per day Database to understand whether songs traveled a certain pattern such as geography.

## Database
https://www.kaggle.com/edumucelli/spotifys-worldwide-daily-song-ranking

Spotify’s Worldwide Daily Song Ranking data source allowed us to work with song rankings and stream counts, ranging across over a year’s worth of dates and multiple countries throughout the globe. 

## Objective/Hypothesis
We were wanting to see if there was a travel pattern of how top hits move throughout the globe. (i.e. does a certain song become #1 in US, then in Italy, then in Great Britain etc) 

What songs are ranked high throughout the year and in what countries?

![Geography Image]

(https://github.com/mansimajithia/Project-1/blob/master/Geography_Despacito.png)

## Data Exploration and Cleanup

* Changed date column to datetime data type instead of object (showed that by df.info() and seeing Date change) because we realized we couldn’t manipulate the actual dates unless it was changed and we wanted to sort data frames by date.
* Dropped URL column and renamed some of the columns to make it more user friendly
* Used ‘global’ region category to find top songs, but then removed global from data set for totals of streams in all the countries because we weren’t sure where the global stream count on a given day came from and did not end up being the same as total of all the countries on a given day
* Mainly looked at songs ranked 1-5 and dropped the lower ranked songs
* Removed columns with no information

## Analysis Process

* Sort functions; how we got the graphs
* Used excel to see if there were any overarching trends
* Broke down data into quarterly sections, per person. Each person took a song and a quarter so that we could find additional trends. We then took multiple songs * and combined our quarterly results. 

## Challenges

* After mining through the data, we realized that we weren’t seeing any patterns we were hoping for, this forced us to change our approach and the breakdown. 
* We struggled with how we were going to create new data frames from the original data for optimal results - to figure out whether we could prove or disprove our hypothesis with the data given. 
* Since the data was taken from the end of 2016, through 2017, and into the start of 2018, we decided to only look at the months throughout 2017, to work with a full and precise year. 
* Meanwhile we realized that the release dates of songs needed to be taken to a high consideration to explain the shift in streams and ranking over time(if a song was released mid year then it would not have data in the beginning of the year).
* It made sense to break the data in quarters so we can look for a trend, while at the same time keeping release dates in mind. We split up by quarter to work more efficiently(4 quarters), here we realized that songs stay popular for about 3 months by streams.
* After splitting up into quarters, we also realized that we need to work over a span of more months to actually show the increase and decrease in popularity, from both sides.

## Conclusion

After working through our challenges, we came to the conclusion that our hypothesis was disproved - the trend of a song didn’t follow any geographical path, and it was difficult to conclude any geographical trend. However, we did realize that the number of streams were typically greater during a specific few months, which brought us to the conclusion that songs stay popular for about 3 months and then die out. 

![Yearly Graph]
(https://github.com/mansimajithia/Project-1/blob/master/Yearly.png) 

