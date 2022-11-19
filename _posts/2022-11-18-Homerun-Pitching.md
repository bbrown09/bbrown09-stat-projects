---
layout: post
title:  "Homerun Pitching"
date:   2022-11-18
author: Bradley Brown
description: Have pitchers gotten better recently or have hitters just started thinking outside the park? Let's explore together!
image: /assets/images/Homerun.png
---

One of the most captivating parts of a baseball game is when a player hits the ball over the outfield fence. Although most baseball watchers would probably say there aren’t enough homeruns to make the game as interesting as they would like, I personally prefer to see pitchers dominate the plate. Because of this, I wanted to look into the stats of the pitchers who had played the most games over the past 8 years and see how their stats impacted the hitting game, especially when it comes to homeruns. 

Before The Pitch

Before I got into my exploratory data analysis, I double checked my data that I had collected and made the decision to cut 2020’s data due to covid limiting the number of games that year. I also realized that when you choose the top 25 players every year based on number of games played, that actually rules out starting pitchers, thus making the complete games and shutouts stats essentially worthless. 
  
Getting into the Data
  
I started by checking the trend of homeruns over the years to see if there had been any general trend or change in the number of homeruns since 2013 by using a regression plot and plotting a line of best fit. As you can see below, the number of homeruns per year seems to have gone up. Does this mean that pitchers are getting worse? Supposedly if we are looking at the pitchers who have played the most games, surely they must be among the better pitchers if their coaches keep letting them play.
  
  ![/assets/images/1_f2-zeAOSNB4RGlqH9emTlQ.jpeg
](https://raw.githubusercontent.com/bbrown09/bbrown09-stat-projects/main/assets/images/Homeruns_By_Year.png)
  
Let’s do the same thing and look at hits over the years to see if our pitchers got any better in this other important category. If you look below, you might be surprised to see that there’s actually an ever so slight downward trend in hits per year. 
  
  ![/assets/images/1_f2-zeAOSNB4RGlqH9emTlQ.jpeg
](https://raw.githubusercontent.com/bbrown09/bbrown09-stat-projects/main/assets/images/Hits_By_Year.png)
  
It seems that pitchers have sacrificed one important stat for another. But just for the tie breaker lets look at the most important stat in baseball: whether or not the other team actually scored on them. To do this we look at ERA which considers how many runs a pitcher actually gives up as opposed to runs given up to his teammates playing poorly. 
  
  ![/assets/images/1_f2-zeAOSNB4RGlqH9emTlQ.jpeg
](https://raw.githubusercontent.com/bbrown09/bbrown09-stat-projects/main/assets/images/ERA_By_Year.png)
  
The tiebreaker appears to go in the favor of the pitchers actually being slightly worse it seems because they are giving up more runs on average even if other numbers might suggest otherwise. Does this mean that hitters are just adapting to better pitching? If we look at the number of strikeouts per year, those seem to go up. The theory I tend to agree with is that pitchers have gotten better overall, plus the defense has started to use statistics to shift field position and make it harder for players to get regular hits, so batters have started to swing for the fences more to guarantee points and a hit. Thus, they get more strikeouts trying too hard to hit homeruns. 
  
  ![/assets/images/1_f2-zeAOSNB4RGlqH9emTlQ.jpeg
](https://raw.githubusercontent.com/bbrown09/bbrown09-stat-projects/main/assets/images/Strikeouts_By_Year.png)
  
Lastly, I thought I’d look at how much homeruns actually impacted wins or saves. It seems like for both stats, the average hovered around 6 HRs for the whole year but went gradually down depending on how much success the pitcher had. Imagine pitching in 74 games like Steve Cishek in 2021, only giving up 2 homeruns all year, and not earning a single save or win. He seems to be an outlier luckily. 
  
  ![/assets/images/1_f2-zeAOSNB4RGlqH9emTlQ.jpeg
](https://raw.githubusercontent.com/bbrown09/bbrown09-stat-projects/main/assets/images/Homeruns_Compared_to_Saves.png)

  ![/assets/images/1_f2-zeAOSNB4RGlqH9emTlQ.jpeg
](https://raw.githubusercontent.com/bbrown09/bbrown09-stat-projects/main/assets/images/Homeruns_Compared_to_Wins.png)
 
And on a similar note, here is an interesting graph showing how often pitchers converted their save opportunities into actual saves.
  
  ![/assets/images/1_f2-zeAOSNB4RGlqH9emTlQ.jpeg
](https://raw.githubusercontent.com/bbrown09/bbrown09-stat-projects/main/assets/images/Saves_Vs_Save_Opportunities.png)
 
Conclusion
  
As you can probably tell, these stats really want to tell us their story, but it is up to us to find it. I think pitching is the best it’s ever been, but as we’ve seen here, it might not actually be. If you want to see the code for these graphs or others I made while doing this research, feel free to check out my GitHub page [here](https://github.com/bbrown09/Pitching_Stats_Project). Let me know in the comments below what you think this data is trying to say and check back soon for a future blog post on what I think this data is conclusively trying to say. 
