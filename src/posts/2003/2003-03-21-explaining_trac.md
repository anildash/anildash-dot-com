---
title: explaining trackback
slug: explaining_trac
date_published: 2003-03-21T21:55:03.000Z
date_updated: 2003-03-21T21:55:03.000Z
tags: weblogs
---

After noticing that both [David](http://www.hyperorg.com/blogger/mtarchive/001332.html) and [Doc](http://doc.weblogs.com/2003/03/18#methododdities) were having trouble understanding TrackBack, I tried to write up a brief explanation, as I understand it, of how the protocol works. Since it was of use to them, I thought I’d repost it for any others who remain confused.

Hopefully I got it right, or else I expect [Mena](http://www.dollarshort.org) will come over here and correct me in the comments.

> Just noticed you said you were still a bit in the dark about TrackBack. If that’s still the case, I think I can explain it to you simply. TrackBack’s just a protocol for one web server to talk to another. The problem is, people have confused the protocol for one of its implementations.

> Right now, the main use of the protocol is to have someone else’s web server tell yours about a message that’s been posted. My server says, “Anil wrote about your post on Thursday.” That works basically like remote comments, and maybe even ought to be displayed the same way that comments are, only linked to the remote site instead of displayed inline.

> Another use of TrackBack, which is just starting to catch on, is for everyone writing about a topic to ping a central place with their comments. These category-based or aggregating TrackBacks are *great*. Imagine a TrackBack-enabled centralized category system, where any post that people on the system make to their “music” category gets pinged to a central music category page. You’d have all the blog entries of all those people, all in one place, by topic. Maybe you could filter it using OPML and FOAF to just those people who are 2 degrees away from your blogroll. Cool stuff.

> Examples of category-based TrackBack aggregation pages:

> [
> 
> notes from people who were at SXSW this year](http://www.sxswblog.com/exchange.asp)
> [
> 
> a similar thing for the ORA OS X Con last year](http://www.movabletype.org/osxcon/)
