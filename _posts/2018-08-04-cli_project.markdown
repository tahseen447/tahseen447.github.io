---
layout: post
title:      "CLI Project"
date:       2018-08-04 09:21:08 +0000
permalink:  cli_project
---


For my first project I chose to scrape https://www.meetup.com/. The idea was to give the user options to choose a category from the list of activities the user might be interested in, then find an upcoming meetup in the neighborhood based on that category.
Like i read in most blog posts, the starting was the most difficult because I was given a blank slate and had to work my way up.
Thankfully avi's video on DailyDeals(https://www.youtube.com/watch?v=lDExWIhYKI) really helped. But I really think that this lesson really helped me through to set up my git repo and commit and play with it.(https://learn.co/lessons/git-basics-mod-set-remote-and-push)
So, I started out ok. Set up my CLI first and was using mock methods and stubs to get the real feel of how my app's CLI would look like.
After I set up my CLI I jumped to scrape the website. Scraping categories wasnt so hard at all and Nokogiri was able to get the nodes that i needed.
The next page was really difficult. I spent a lot of time figuring out why Nokogiri couldnt get the nodes that i was requesting. It worked the first time so why not now. After setting up 1:1 with a coach, we figured that the data was being rendered from JAVASCRIPT and so Nokogiri cant acces that. Enter Poltergeist(https://readysteadycode.com/howto-scrape-websites-with-ruby-and-poltergeist). We played around a bit and discovered this will get me the javascript nodes i need to scrape the activites related to a particular category. 
Then ofcourse there were issues. I ran into exceptions from Poltergiest. In order for the app to not break, I had to write some exception handling and yes that needed some research work and another 1:1 session from coach.
Everything else seemed to work after ofcourse picking at it whenever I was stuck.
There is sitll something that we havent figured out why. So the app scrapes the website and returns upcoming meetups in the neighborhood, so in chrome browser I can see activities 5 miles of Los Angeles, but in nokogiri, it fetches the data of the Bay Area(Like Cupertino. CA)
The theory is chrome and nokogiri use some browser data that is set differently for both these url requests and so the difference. But I'm still open to any suggestions as to why this may be the case. Overall, good work. And yeah , here's the record walkthrough.
https://youtu.be/q279K5FOZxM
