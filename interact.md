---
layout: default
---

# Does the users interact with each other?

This was one of our research questions, and a lead where it was possible to find some patterns in whether one can detect if a user is a troll.
If you want to skip to that part, click [here](./userdetect.html).

## Distribution of all users

![DIstribution of the users that interact and have interactions](/interacting/allusersdistributionmain.png)

> Disclaimer: The number of users that have been interacted with by others are skewed in this plot. The green bars could and should probably be a little bit higher, especially remarked in the bucket (0,10]. This is because the number of times a tweet is retweeted, quoted or replied to is wrong a few places. Check out our [notebook](link) if you want to learn more. The blue bars still account for what it is meant to be.


- Most users tweet under 500 times, but the difference is not is not very huge between users that have tweeted less than 500 times and users that have tweeted over 500 times.

- There are a fraction of users that have tweeted in such small numbers, so the impact of them is very small. Here we can see that the more tweets the users have the more likely it is that interactions with other trolls increases as well, which is natural. 

- The most interesting aspect is probably the mastodonts that have tweeted over 10000 times. These users have been interacted with by other trolls much more than interacting to trolls themselves. This is strange, given the large amount of tweets which makes it more likely to have interacted with anyone. This differs significantly from the user with between 1000 and 10000 tweets as well. In general, the higher tweet count the more even the three bars would be, as it seems that this is the natural way the relationship between the three bars evolve.

## Cumulative distribution of how the trolls interact to other trolls

![Cumulative distribution](/interacting/cumulativeinteracting.png)

To interpret this visualization:
- This mean that almost 20% of the trolls have never interacted to trolls.
- 50% of the users have more than 30% of their interactions directed to trolls, and 50% has less than 30%.
- Around 30% of trolls have more than 50% of their interactions directed to trolls.
- Around 5% of the users only interact with trolls.

In conclusion, yes they do interact with each other, and some of them does it a whole lot. As we saw in [how we made the tag of bot-likely users](./botdeciding.html), many users also tweet exactly the same content as well, meaning that users also are connected in other forms than through interactions.

Since many of the trolls so clearly is interacting as an unit, we divided them into a whole bunch of categories to try to find out how normal users could detect them.

> Since the user with under 10 tweets are almost invisible to most of normal Twitter users and only half of them have ever interacted as well, we remove them for the main categorization of users. Most people will never even see those trolls, and users that never get more than ten tweets will in general been questioned as being a significant Twitter user at all.

> Therefore the next analysis will contain users that have a minimum of capability of impacting the general discussion, since they are or have been active at all, with that definition only being reaching a number of over 10 tweets.

More on this on [this page](./userdetect.html).

***
*Was this interesting? Check out our other analysis:*


- *[Read the general statistics of the trolls? It might give you more insight to this page!](./generalstats.html)*
- *[Read about how we found the bot-likely patterns.](./botdeciding.html)*
- *[Can normal people detect the russian bots?](./userdetect.html)*

[Back to start page](./)
