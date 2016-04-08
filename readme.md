#Twitter Oversight Dashboard

## Idea

My idea is to create a dashboard that allows me to spot and mark power outages around the Netherlands, this will be done by collecting certain tweets containing keywords like #stroomstoring #geenstroom etc. In addition, I will grab all the geolocation settings this tweet has, and place a marker on a map. With several markers in place, I can draw an area that should contain the rought area in which there is no power left.

## Data sources

I will be using the Twitter API to collect data from Twitter. This API is one of the most sophisticated API's in the world, and after exploring the options, I should be able to use this API in conjunction with meteor to update the variables in real time. I'll have to develop an algorhythm as well to find a balance between false positives and / or fake geolocations.

## Optional

I want users to be able to filter certain keywords, users, tweets, or to filter locations. I also want to give users the option to use their own Twitter account to do these requests themselves (API Rate Limit reduction) so they can track their own sentiments. This dashboard could also be used on a wider scale (elections, major sport events) to track metadata about the general sentiment / emotions.

I like this plan, you better not submit mean issues to break my idea.... ;)