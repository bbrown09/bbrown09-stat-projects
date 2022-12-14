---
layout: post
title:  "From the Plate to the Left Field Fence: A Journey by Data"
date:   2022-12-08
author: Bradley Brown
description: This is the story I was able to tell from the Pitching data I collected.
image: /assets/images/HomerunHitter.jpg
---

How We Got Here

  Every good story has a beginning, and this one begins a love for sports, especially baseball. I needed to make a blog, and as a huge sports enthusiast, I thought it would be quite appropriate to focus on baseball stats since I’ve looked at football stats and basketball stats for previous projects. When I began this project, the Major League Baseball Playoffs were right in the swing of things and Aaron Judge had just broken a long-standing record of homeruns in a season for the American League. This led me to wonder why this old record had been broken. Was it just improved hitting or worse pitching? Maybe a little of both?
  I decided I would look into it by looking at pitching stats of the most frequently played pitchers of the last 8 years. I was able to get the stats I needed right from MLB.com. With a little bit of scraping and combing of stats from different years, I was able to get the data of roughly 200 pitchers. With that data collected and compiled, I moved on to exploring the data through different graphs and plots. You can read about these steps in my other blog posts [here](https://bbrown09.github.io/bbrown09-stat-projects/), and you can look at the code that I wrote to collect and explore that data [here](https://github.com/bbrown09/Pitching_Stats_Project).
  
The Data Story
  
  After studying the data and visualizations with my question in mind about what helped Aaron Judge to break the homerun record this year, I believe I have found the story that this data is trying to tell. It would be easy to say that Aaron Judge is just a generational talent when it comes to hitting homeruns, and that is probably also a little true, but as we look at the trends of homeruns given up over the years by pitchers compared to strikeouts, we can see an obvious trend of strikeouts going up as well as homeruns. To me this says that neither pitchers or batters are getting better or worse overall. Instead, an outside factor is influencing the game. My belief is that the culprit is actually the shift by the defense. Recently defenses have been using statistics to move to the parts of the field where batters are most likely to hit. This makes it harder to hit base hits, so batters are forced to improvise or hit it right to the defense. Ultimately, the swing for the fences mentality was created, or more likely, grown more noticeable. Batters swing more out of control which rewards them with more homeruns, but also more strikeouts. Thus, a new homerun king was born.

{% include Homeruns2013-2021.html %}

{% include Strikeouts2013-2021.html %}
  
Conclusion

This project has been quite fulfilling for me to finally finish. Hopefully you learned as much from reading it as I did from writing it. Let me know if you agree with my conclusions in the comments below or tell me about a data story you have discovered for yourself. If you are interested in any of my code, check out my repository [here](https://github.com/bbrown09/Pitching_Stats_Project). Thanks again for reading!
