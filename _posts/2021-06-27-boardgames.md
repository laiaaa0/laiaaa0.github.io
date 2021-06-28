---
layout: single
title:  "Boardgames"
date:   2021-06-27 11:23:23 +0100
categories: python
---

I spend quite a lot of time playing boardgames. Although I won't research new games, and have never financed kickstarter campaigns, I enjoy spending afternoons and evenings playing boardgames with friends.
When the pandemic started, I immediately bought [tabletop simulator](https://store.steampowered.com/app/286160/Tabletop_Simulator/) on steam so that I could continue to play boardgames with friends. I currently have 192 hours played, so I would say it was quite a good investment.
Now that things are starting to open up in the UK, I have been playing face to face again, which makes it a lot more enjoyable. 

During a boardgame conversation with my partner, the idea came up to play the top 100 games on [boardgamegeek](https://boardgamegeek.com/), the reference site for boardgames. Then, we would rate each of them and see how similar our ranking is to the one on the website.
Since I wanted a spreadsheet with the list of games, their rank, and some additional data, I went and created a python script that would parse the boardgamegeek website, and output a csv file that contained all the information I needed. 
This was a great way for me to procrastinate from the rest of the work I had to do last week.

For the script, I used HTMLParser to parse the HTML from the website, and defined a class for each row in the list. 
Then, whenever I found a new table row I would create a new row object, and whenever I found a table data cell I would fill that field from the current row object. After parsing the full HTML, I saved all the information as a csv, row by row. Since I coded this in a fast and sloppy way the code is not documented, but I'm happy to answer any questions about it.
You can found the full script [here](https://gist.github.com/laiaaa0/61fc9e45bbff7e4a41fa675ffda9d547). 

