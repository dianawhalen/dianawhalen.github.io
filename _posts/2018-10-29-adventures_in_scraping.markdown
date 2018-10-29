---
layout: post
title:      "Adventures in Scraping"
date:       2018-10-29 15:01:06 +0000
permalink:  adventures_in_scraping
---


The CLI Data Gem Project was certainly an interesting one...

When I began this project, I selected a site that was both structurally sound (as far having a consistent site architecture, and minimal use of scripting, as per project guidelines), and one that represented my personal interests (indie game development). 

I had done a significant amount of work on my project, when I received a mass email communication from the site founder, announcing he had made the decision to shut down the site after years of operation, so that he may direct his focus elsewhere. 

In some ways it was fortunate that I happened to be a member of the site, and thus received this email, alerting me that I had two weeks before the shut-down date.

At that point, being reluctant to lose all the progress I had made, I decided to download the site, and just make use of it offline, as fixtures in my project directories. 

What I didn't anticipate however, was just how many files and data the site hosted, seeing as it was largely made up of images, so downloading the entirety of it became a significant undertaking, not least of which was managing the disk space to accommodate it.

After several more obstacles presented themselves in my efforts to continue on this path, I made the decision to start over with my project. A fresh start with a fresh site.

I chose a site that was similar to my initial one, for the same reasons, being a desirable and manageable site architecture, minimal use of scripting, and a reflection of personal interests (this time around, web & graphic design projects).

What I found intereting (though unsurprising) throughout the process, is the degree to which a site may have many small changes made continuously, in order to make it more usable, and better organized. 

While this is of course a great benefit to a user's experience in navigating a site, it highlighted a need to frequently make even minor updates to my code, in the methods I created to scrape the content from the site. Of course, this should be expected when dealing with any dynamic source of data.

Although I approached this project with the intent of creating and publishing a Ruby Gem (and did create my application as such), it was clear to me that this approach would probably be best left to sites that utilize very consistent and universal types of site structures, and that the data desired from them be significant in volume. 

Seeing that sites fitting this description often have APIs available to obtain this information, the specificity of many sites, or what might scrapable from them might not make for the best Gem candidates. 

That said the process of learning how to create one, has been valuable, and I plan on fleshing out several ideas for Gems I wish to create in the future.



