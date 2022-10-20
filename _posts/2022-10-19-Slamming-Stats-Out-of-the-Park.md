---
layout: post
title:  "Slamming Stats Out of the Park"
date:   2022-10-19
author: Bradley Brown
description: Have you ever seen Moneyball? This is my attempt to become like Brad Pitt's character and find the stats that impact baseball the most.
image: /assets/images/Moneyball-your-supply-chain-1280x720.jpg
---

	For anyone interested in sports even a little bit, October is easily recognized as the best month for these games we love. Basketball is starting its season, football is about halfway through its own season, and of course there is plenty of soccer to go around as well. Most importantly though, the Baseball playoffs start and end in October with the World Series capping off another season of America’s pastime. This of course makes me want to do whatever I can to dive into the stats of Baseball, particularly its pitching stats as they are the most intriguing to me. 

America’s pastime

There are plenty of choices when it comes to stats and baseball, but the category that appears to me to affect the game the most are the stats concerning the pitching. In the past few years, it has become harder and harder for hitters to hit the increasingly crafty and speedy pitches that are being thrown. All you have to do is look at the increase in average pitch speed and decrease in batters’ averages. According to some experts, the average major league fastball has improved 3.8 miles an hour in the past 20 years.

![/assets/images/1_f2-zeAOSNB4RGlqH9emTlQ.jpeg
](https://raw.githubusercontent.com/bbrown09/bbrown09-stat-projects/main/assets/images/2022-10-19.png)

Deciding which stats to use

I wanted to see if any other factors played a part in the decline of batters and the rise of batters, so I figured I would look at the stats of the top 25 pitchers through the past 8 years. The best place to get stats like that are from MLB.com. I just decided to use their main 19 stats for my initial data scrape and analysis. For those who might not know about these stats, click [here](https://www.mlb.com/glossary/standard-stats) to learn more.

The actual Scrape

In order to actually get the data, I decided to use Beautiful soup and requests to manually pull the data myself. Although most official sports websites data is legal and free to scrape, I double checked that this was ok by doing the following code and making sure I got a 200 result which just confirms that there’s no blocker on the data.

```
page.status_code
```

Since there was 8 different pages, I manually updated the code by 1 number every time to grab the different pages I needed. The results were great after I combined my data altogether. You can check out the data in my repository as well as the code to scrape it [here](https://github.com/bbrown09/Pitching_Stats_Project).

Conclusion

Baseball has changed a lot over the years, but with each change the game has gotten better. Thankfully, the world of stats has gotten even more in depth right along with it. Check back in on my blog soon to see my attempt to start analyzing this data that I have collected. Let me know too if there any stats you’re particularly interested in seeing if they affect the game or if there is another sport that you are more interested to find out about. I’d love to chat with any fellow sports fans!
