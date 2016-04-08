#Twitter Oversight Dashboard

## Idea

My idea is to create a dashboard that allows me to spot and mark power outages around the Netherlands, this will be done by collecting certain tweets containing keywords like #stroomstoring #geenstroom etc. In addition, I will grab all the geolocation settings this tweet has, and place a marker on a map. With several markers in place, I can draw an area that should contain the rought area in which there is no power left.

## Data sources

I will be using the Twitter API to collect data from Twitter. This API is one of the most sophisticated API's in the world, and after exploring the options, I should be able to use this API in conjunction with meteor to update the variables in real time. I'll have to develop an algorhythm as well to find a balance between false positives and / or fake geolocations.

## Feature path

 - Create a working HTML/CSS based meteor dashboard without data.
 - Ensure I can use the Twitter API to communicate with twitter.
 - Have the application contact the API to request the latest tweets.
 - Apply an algorhythm to differentiate the tweets.
 - Apply groups of tweets into confirmed, possible and false positives.

The above system should be enough for a minimal viable product, but I think the upcoming points should be possible as well.

 - Check for geolocation. And if available, load geolocation into a map.
 - Update the map with a polygon that connects a possible or confirmed group of outtages.

## Twitter API

The Twitter API has an extensive amount of search query's. Most importantly the search/tweets one. This API works like:

 - Response formats
JSON
 - Requires authentication? 
Yes
 - Rate limited?
Yes
 - Requests / 15-min window (user auth)
180
 - Requests / 15-min window (app auth)
450

I can select the since_id to skip previous results, and give a maximal amount of returns by changing max_id.

## Optional

I want users to be able to filter certain keywords, users, tweets, or to filter locations. I also want to give users the option to use their own Twitter account to do these requests themselves (API Rate Limit reduction) so they can track their own sentiments. This dashboard could also be used on a wider scale (elections, major sport events) to track metadata about the general sentiment / emotions.

I like this plan, you better not submit mean issues to break my idea.... ;)
