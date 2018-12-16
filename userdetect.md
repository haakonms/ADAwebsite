---
layout: default
---
# Can a normal person detect whether a Twitter user is a troll?
In general, the answer to this question is no, unfortunately. Most Twitter users do not have time, or don't take the effort to detect some of the trolls. It is impossible to separate the Russian trolls from other trolls, but you may be able to detect whether this user is a troll in general! To do this you need to know some about the different categories of trolls.

This is a table showing the numbers and percentage of different user categories in the dataset. Do they have traits that makes it possible for us to detect them?

![Table with all the categories](/categories/finaltable.png)
> The empty cells have no values.

## Trolls that never have interacted at all
![Non-interacting users and likely bots](/categories/non-interacting.png)
### Non-interacting regular users:
> Regular users is total users minus likely bots. 
- Around 4.7 % of the users in the dataset. They have few followers and do not tweet much. You will probably never be in touch with these since they have such small impact on the overall discussion on Twitter. How can you detect these as trolls? There is probably nothing special about their tweets and can not be detected by just looking into the profile or tweets, but one could try to reply to one of their original tweets with a question if you suspect a troll and see if it answers


### Non-interacting bots: 
- Around 8,3 % of the dataset. They have exclusively few followers and have a medium amount of tweets, but never more than 2500. These are probably the easiest to detect. You could easily search for the same content (take something with a significant length) in the Twitter search option and find numerous other encounters of the same tweet. You could also look at its feed and see that it has a really monotonic way of tweeting. In addition you could also apply the same tactic as over and wait for an answer, though it might be that some of them have the feature of answering. Try asking a complicated one in that case.

## Trolls that mainly interact with other trolls when they interact.
![Mainly troll-interacting users and likely bots](/categories/mainlytrollinteracting.png)
### Mainly troll-interacting regular users: 

- Around 15,3% of the dataset. Mainly pretty evenly distributed, but few of them have many followers, though they make up a good amount of the users with most followers. They have a average amount of tweets. If you are able to know whether other users are trolls, you could find patterns in this users way of interacting with others. As a normal Twitter user however, it seems rather hard to tell if it is in this category. These users mainly have not a big outreach, but among the user with most followers they are very effective for their purpose by exploiting the fact that they have many followers to advert for other Twitter trolls and make them more noticed by retweeting and quote tweeting. This probably makes them one of the more dangerous categories.


### Mainly troll-interacting bots: 
- Around 11% of the dataset falls in this category. Has a medium distribution of total tweets, never over 2500. Always a low amount of followers, almost exclusively under 200. One can use the same tactic as with all bots, search for their original content and look for numerous other encounters. Again it would be difficult regarding whether you know how other users are trolls, but since they make up around 50% of all interacting bots with under 200 followers, this may be a way to detect other twitter trolls.

## Trolls that most of their time interact with other users.
![Highly interacting users and likely bots](/categories/highlyinteracting.png)
### Highly interacting regular users:
- Around 20% of all users in the dataset are in this category. There are a small amount of such users in the medium range (100 to 1000) of total tweets. They make up a significant number of the trolls with a small amount of tweets, as well as a semi-high amount of users around 2500 to 5000 tweets. Those users are hard to detect as trolls compared to other users that interact a lot, but you should have a natural skepticism towards users that mainly tweets by forwarding other messages in form of retweeting and quoting. 

- In case of followers most of them have medium amount of between 100 and 500, but are represented in all the ranges. Some of them may be retweet bots that convey a specific political standpoint, but overall it is users that would avoid being recognized as trolls.


### Highly interacting bots: 
- Around 9.7% of all users in the dataset are in this category. Exclusively have more than 500 tweets, mostly over 1000. They always have a high amount of followers, mostly being between 500 and 7500 followers where they make up over 50% of all interacting users. 

- Since they have so specific common traits, these users can be picked up as trolls if you have a keen eye. Look for their original content and check whether it is duplicates using the same methods as earlier mentioned 

## Trolls that are highly interacting and mainly interact to other trolls.
![Highly interacting non-bots that mainly interact to trolls users and likely bots](/categories/hiahta.png)
### Highly interacting regular users that mainly interact to trolls: 
- This category is an overlap of the two abovementioned categories. Around 4% of all users in the dataset is in this category, and 4 percentage points of the users in each the categories over except none-interacting users. They are pretty evenly distributed in terms of both total tweets and followers. The same yields for these users as the two mentioned in case of detection. They are slightly easier to point out, but unfortunately, it is still hard for a common Twitter user.


### Highly interacting bots that mainly interact to trolls:
- These users do not exist so far. Probably because it easily could be picked up on by algorithms if the only thing you do as a Twitter user would be to interact with only a specific number of users with a bot-like pattern.

## Trolls that so far does not have a category.
![Non-categorized users and likely bots](/categories/noncategorizedusers.png)
### Non-categorized non-bots: 
- Around 18,1% of all users. They do have the traits that the other categories don’t have, but this only makes them looking like normal twitter users. They are evenly distributed in terms of both total tweets and followers, but they make up the majority of total users with more than 10000 tweets and 7500 followers. This means that these users are the ones that has the most impact on the general discussion on Twitter, and reaches the broadest amount of people.
 
- It is very likely that these are the users that are seen by IRA as the main communicators of opinions, and have a very high chance of being fully controlled by real humans, as we know a number of the users are. This [article](https://www.buzzfeednews.com/article/maxseddon/documents-show-how-russias-troll-army-hit-america)  provides insight in this claim.


### Non-categorized bots:  
- Around 16,4% of all users. They rarely have more than 2500 tweets but account for around a third of the users between 1000 and 2500 tweets. In terms of followers they are mostly limited to under 200, and do not exist in the group of users with over 7500 followers. Unfortunately, there is no way to detect these users except the method that applies for all bots. Search for their original content of significant length, and look for numerous duplicates.

All users are now more or less categorized, and some of them is possible to detect. What they do have in common is again their likeliness of being bots. If we look at all the categories we have created that includes bots and compare them together, we can observe an extraordinary distribution in between.
![Follower and tweetcount](/botsdeciding/botinteracting.png)
* The likely bots almost has a perfectly dividing line in both followers and tweet count. Almost all of the likely bots that interact at all are mainly interacting bots. The same accounts with the bots that interact at all over 500 followers.

* This means that the likely bots that mainly interacts with other users tweets an enormous part. They also have a lot of followers which we may suppose that comes from the extreme amount of interacting with other normal Twitter users. They may also have bot-like behaviour when it comes to following others. 

* The fact that he bots that mainly interact with other trolls has a small amount of followers is not surprising since they mostly don't reach out to other users and tweet in limited numbers.

Detecting Twitter trolls is not an easy task, but know you have some pegs to put the different users on. Applying this in daily Twitter use will however be difficult and time-consuming. Good luck!


***
*Is this your last page? If not, check out our other analysis. A lot of this page is based on other interesting information.*

- *[Read the general statistics of the trolls? It might give you more insight to this page!](./generalstats.html)*
- *[Does the trolls interact with each other?](./interact.html)*
- *[Read about how we divided the users into bots and regular users!](./botdeciding.html)*

[Back to start page.](./)
