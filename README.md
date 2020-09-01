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

When approaching the hypothesis we were trying to look at a specific song and look at how it travels throughout the globe when it hits top 1 in each country. After looking at multiple different songs we sorted the data sets of each song by date and then looked at the date that it first hit number 1 in each country and dropped the rest of the data. We noticed that there was no pattern in how a song travels but decided to look at some other questions about the timeline of a song with our data. These two graphs above show how each song is ranked geographically by date. Each song is popular regardless of region at the beginning of the date. There is no discernable trend that the song travels. The regions at the end of the date are in the same geographical regions as those early on. 

* What did the timeline of a song look like?
* Each song lasted roughly for a few months, it seemed to peak in one month but was still in the top during the surrounding months. 
* Specifically, certain songs become popular during different seasons depending on their release date, during the holiday months the holiday songs seem to knock other new music off the top charts and take over with an overwhelming amount of streams.


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

## Implications of Findings
We unfortunately didn’t find what we expected to find - which was some sort of travel pattern, where we could see how song popularity travels around the globe. But we did find that songs stay popular for a certain period of time, and this brought us to the idea that maybe these songs are staying popular during a certain few months because the type of song relates to the timing of the year? This got us thinking further - does the genre and mood of a song reflect what season it is most popular in? These questions will allow us to further analyze this data with new ideas and goals - we can look for different trends and conclusions. 
