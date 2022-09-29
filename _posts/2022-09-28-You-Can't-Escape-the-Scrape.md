---
layout: post
title:  You Can't Escape the Scrape!
date:   2022-09-28
author: Bradley Brown
description: A short tutorial to help you run towards scraping data from the internet using R rather than away from it.
image: /assets/images/1_f2-zeAOSNB4RGlqH9emTlQ.jpeg
---

What is the most essential part of doing work in the field of statistics? Having good data of course. While it is possible to collect your own data and make your own data frames for your work, it is much easier to build on the shoulders of those who came before. The internet is full of data that has already been collected and is just begging to be analyzed by us statisticians. I remember I avoided scraping data from the internet like the plague when I first started statistical work. It was intimidating, but eventually I could no longer escape the need to scrape date from the internet. Once I learned how to do it simply, it was no longer something to fear, but something to look forward to. Thus, today I will give a short how-to when it comes to scraping data from the internet using R.

The first step for any coding project in R is to load up the correct libraries. In this case, the library we need is called “rvest”. If you don’t have it, make sure to use:
```
install.packages(“rvest”)
```

Next, find the url of the website you would like to scrape the data from. Since I’m a huge basketball fan, I’m going to show an example scrape where I pull the top 25 scorers of all time for the NBA from ESPN.com. 

```
top_scorers_url = read_html("http://www.espn.com/nba/history/leaders")
```

As you can see, I used the function “read_html” to assign the url to the variable I’m calling top_scorers_url. Once you have this completed, its time to learn how to read html code. Go ahead and right click the table or container you would like to scrape your data from. Look for the option at the bottom called “inspect”.

![/assets/images/1_f2-zeAOSNB4RGlqH9emTlQ.jpeg
](https://raw.githubusercontent.com/bbrown09/bbrown09-stat-projects/main/assets/images/2022-09-28.png)

This will open up the code working in the background to produce the web page you are viewing. Hopefully, you right clicked your table correctly and it takes you to the right spot in the code where the data you want is stored. Most of the time this data will be labeled “table”, but if not, scroll your mouse over the code until the data you want is highlighted on the web page. This is called the html node and it is how we tell our code what to look for. For more information about html nodes and examples of using them in scraping, read here: [nodes](https://rvest.tidyverse.org/reference/html_nodes.html)

![/assets/images/1_f2-zeAOSNB4RGlqH9emTlQ.jpeg](https://raw.githubusercontent.com/bbrown09/bbrown09-stat-projects/main/assets/images/2022-09-28%20(1).png)

Once we have confirmed the name of the html node we need to scrape from, we can use this code (which utilizes piping. For more info about piping check out this page: [pipes](https://r4ds.had.co.nz/pipes.html)) to grab the data and store it into a table.

```
top_25_scorers = top_scorers_url %>%
  html_nodes("table") %>%
  html_table()
```

Notice we take our url variable and perform the functions “html_nodes()” and “html_table()” in order to get our data. Use whatever node you got from inspecting the html code earlier. For many this could technically be a stopping point because you should now have the data you want in your possession. For me though, I prefer my data in data frame form and this method will usually gather the data into Tibbles. Not to mention, if there was more than one table on the page, you might pull in all of them when you just want one.

![/assets/images/1_f2-zeAOSNB4RGlqH9emTlQ.jpeg](https://raw.githubusercontent.com/bbrown09/bbrown09-stat-projects/main/assets/images/2022-09-28%20(3).png)

In order to get a data frame of just the data you want, you’ll need to open the table up, and look at what number tibble your desired data is under. Then based on that number, you just use the code below and replace the one (the index) with whatever number your tibble was. 

```
alltimescorers = as.data.frame(top_25_scorers[1])
```

Your data should now be in a nice-looking data frame that you can mess with as you please. 

![/assets/images/1_f2-zeAOSNB4RGlqH9emTlQ.jpeg](https://raw.githubusercontent.com/bbrown09/bbrown09-stat-projects/main/assets/images/2022-09-28%20(4).png)

If I can scrape data from my favorite sport this easily, think of all the other data out there you could also scrape without fear. Think of all the time you just saved by not having to collect your own data or retype a thousand lines to remake the table yourself. Now go and see if you can scrape data about your favorite topic using these simple steps and never try to escape the scrape again!

