---
title: Twitter, Transclusion and Trust
slug: twitter_transclusion_and_trust
date_published: 2010-09-17T17:02:15.000Z
date_updated: 2019-11-15T22:40:06.000Z
tags: [tech, twitter, web]
---

The new Twitter is here! The new Twitter is here! Besides sowing discontent in our household by giving me access to the new user interface before my wife’s account has been upgraded, the big new feature of the update to venerable old [Twitter.com](http://twitter.com/) is a sidebar that lets you view media that’s been mentioned in a tweet. Videos! Photos! Kickstarteros!

Unfortunately for readers of this blog, I have a years-long fixation on transclusion of hypertext documents. Transclusion is technically defined as “when you put that one thing in that other thing”. In its current implementation, Twitter has declared that media which is shown within the Twitter interface comes from [selected partners](http://twitter.com/newtwitter). But actually, the technology to allow embedding of rich media from almost any site already exists, using a system called [OEmbed](http://www.oembed.com/). Geeky stuff, but it’s made by nice people who are pretty smart, and it lets any site say, “Hey, if you want to put our thing in your thing, do it like this”. It works. Lots of sites do it.

Nobody’s getting rich off of it, but nobody’s getting sued, and in between those two extremes lies most of what makes the web great.

## What Twitter Could Do

So, is Twitter using OEmbed to do its new sidebar media thing? Dunno. It’s unclear. They *probably* are building on top of OEmbed in some way, but if that’s the case, then it hasn’t been documented anywhere.**Update:**[Yep, they are!](http://Twitter.com/noradio/status/24790949420)

But if Twitter *did* declare they were using OEmbed, that would let them say either one of two good options:

1. If your site supports OEmbed, and someone tweets a link to it, it’ll Just Work! (This would be awesome, but tricky.)
2. If you have a site that supports OEmbed, and want it to Just Work in Twitter, submit your link to us in some simple way. (This would be less gee-whiz but still great.)

Even better, if Twitter adopted smart use of OEmbed in this way, and if they went one step further and published the list of services that had registered with them as offering their content up for embedding, we’d have a great registry of all the media that was ready to be transcluded onto other websites. I am pretty sure “transcluded” is a word. I would play it in Scrabble.

That’s a whole new world of remixing the web that has been technically possible, but practically a pain in the ass, and Twitter could catalyze some really fun ways to combine content from different sites. YouTube owes some significant part of its overall dominance in video on the web to its popularization of simple embedding of media in other sites. There have been a few efforts over the years to popularize the embedding of widgets across the web in various ways, but except for promotion (Digg, Twitter and Facebook “Like” buttons) and ads (Google!), they haven’t really caught on in terms of functionality.

There are, of course, little companies and projects doing some of this stuff on their own. [Embed.ly](http://embed.ly/) has a whole directory of different kinds of content they’ll help you embed. [Widgetbox](http://www.widgetbox.com/) is still around, though they predate the use of the omnipresent Libyan domain name suffix. [oohEmbed](http://oohembed.com/) seems nice, though its name wins the cautionary award for why you shouldn’t let coders do marketing, just as you shouldn’t let marketers code.

But none of them has the traction, or the market influence, that Twitter does. If Twitter embraces OEmbed as the way to get into its sidebar in a seamless way, it could finally move this stuff from the esoteric fringes of web hackers into a capability that every media publisher would want to support. Oddly, even some major web widgets we see today, like Google AdSense, don’t support OEmbed for easy incorporation onto other sites. (YouTube and Flickr do.)

## I’m In Ur Blog &c.

For my part, I hope Twitter makes their own ecosystem more open by offering this standard way to get one’s own media built into the Twitter.com experience when someone tweets a link to it. I hope Twitter also allows tweets to be sent *out* through OEmbed, so that it’s easier to embed them (instead of using the casual [Blackbird Pie](http://media.twitter.com/blackbird-pie/) tool they’d thrown together) in other sites. And most of all, I hope more people experiment with seeing how we can combine content from our sites together in new ways. Imagine if someone could just skim previews of your blog posts inline if a friend had tweeted a link to your site. It’d be cool!

To help figure out how this stuff could work, I’ve reinstated the ability to embed excerpts of my blog posts into other sites, and I’ll be watching to see if any interesting results come of that. (I don’t yet support OEmbed for my blog posts here, but if I have time next week, I’ll add that.) A little more background:

- [Embedded Journalism](/2008/03/14/embedded_journalism/): A few years ago, I added the ability to embed an excerpt of my blog post into other sites. It kicked off an interesting discussion.
- [Reinventing Copy & Paste](/2006/03/05/reinventing_cop/): See, I really wasn’t kidding about the transclusion thing. I think it’s a big deal.
