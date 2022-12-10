---
title: Massaging the Data
slug: massaging_the_d
date_published: 2006-07-19T16:30:30.000Z
date_updated: 2006-07-19T16:30:30.000Z
tags: random ha-ha
---

Speaking of [memes from a year ago](http://www.dashes.com/anil/2006/07/18/the_goatse_tshi), last year I created a site called ishavingamassage.com. (That’s “Is Having A Massage”, not “I Shaving…”) The domain is a (gentle) poke at [Flickr](http://www.flickr.com/), which uses the message “Flickr is having a massage.” as its error/downtime message when the service is taken offline for repairs or maintenance.

The founders and several of the members of the Flickr team are friends of mine, so it wasn’t intended by any means to be a dig at the site. (Except maybe for being so lighthearted and cheerful while so many Flickr addicts are panickedly hitting “refresh”.)

At any rate, the massage site had a nice little run for a few months. It acted as a goofy inline link for people to use when making a point in a blog post, or as a little toy for people who like to kill downtime at work by typing in different URLs and seeing what happens. You know, something like [yo.momma. ishavingamassage.com](http://yo.momma.ishavingamassage.com/).

### How it works

For those who’ve never tried it, the behavior is simple. You type in *your.site*`.ishavingamassage.com` into your browser, and it displays a custom Massage Message, coloring the text of the *your.site* part of the address Flickr-style, converting any dots in the URL to spaces, and removing a penultimate “e” character if the last letter of the site name is an “r”. Not rocket science, but it amused me for the hour or so it took to build.

On a lark, I decided to log the massages after the first hour or so that the site was running. I didn’t keep track of timestamps or the IP addresses of people who accessed the site or anything else that might start people fussing about privacy, etc. If I’d have planned ahead, I probably would have thought more about that.

Anyway, the amount of analysis and actual understanding of user behavior that I can do is limited. What becomes clear is that some popular sites really encourage people to click on links, and others that seem equally popular are mostly frequented by people who are less active clickers. Note, I also special-cased one or two websites where the site owners took down their websites entirely and redirected all of their traffic to *sitename*`.ishavingamassage.com`. Those sites were bounced to google.com and the requests weren’t logged, due to volume. Those are removed from the data set.

### The Data

Thanks to [Ben](http://btrott.vox.com/), I was able to crunch the numbers a bit about what things people were massaging. The Top 10:

# kottke: 6843

# flickr: 6412

# jasmeet: 5187

# yanni: 3422

# upcoming: 3012

# my wallet: 2065

# aelki: 1831

# mathowie: 1495

# brice: 888

# arvind: 854

If you’re looking for raw data, I’ve got the log file here: [massages.txt](http://www.dashes.com/anil/massages.txt) (750k plain text file). We’ve also got the raw data of counts, as an Excel file. [massages.xls](http://www.dashes.com/anil/massages.xls) (839k Excel spreadsheet). All of this data is from approximately one month ago; There’s a live data feed, but I’ll link to that later.

![Massages Data](__GHOST_URL__/images/massages.png)

### The bottom line

So, what conclusions can we draw? Jason Kottke is a very popular blogger. And the audience that responds to this kind of web wankery has a fairly high percentage of people who like to try at least some primitive-level hacking. There were a surprising (to me, at least) number of people trying to escape characters or add commands to the script that runs the page, along with a healthy number of people who just wanted to mess up the HTML on the page. There are also a surprising number of people who want to redirect all their traffic to another site for at least a temporary period of time.

Not surprising? Lots of people like to talk about body parts belonging either to themselves, their friends, or various people’s mothers.

Some items that might be of interest:

- Flickr has far fewer massages these days; To understand why, please see Cal Henderson’s [Building Scalable Web Sites](http://www.amazon.com/exec/obidos/ASIN/0596102356/2020-20). Cal’s on the Flickr team, and reveals a lot of his secrets here.
- Rafe Colburn says “[Log it, don’t count it](http://rc3.org/2006/07/log_it_dont_cou.php)“. He’s completely correct.
- The massage site didn’t originally have ads on it. I put them on now since I believe you should start paying rent after you graduate.
- I got through this whole post without mentioning power laws or the Long Tail! Aw, crap.
