---
title: The Twitter API is Finished. Now What?
slug: the_twitter_api_is_finished
date_published: 2009-12-18T17:27:27.000Z
date_updated: 2009-12-18T17:27:27.000Z
tags: Most Popular, tech
---

**Update:** We’ve got some results already! Joseph Scott at Automattic mentions [in the comments](http://dashes.com/anil/2009/12/the-twitter-api-is-finished.html#comment-661931) that he’s added RSD support for the Twitter API to WordPress.com. I should also make clear that I am very confident that we’ll be building apps on top of this API at [Expert Labs](http://expertlabs.org/), so insofar as I’m the Director of the labs, I’ve got a vested interest in seeing efforts around an open API succeed.

---

Twitter’s API has spawned over 50,000 applications that connect to it, taking the promise of fertile APIs we first saw with Flickr half a decade ago and bringing it to new heights. Now, the first meaningful efforts to support Twitter’s API on other services mark the maturation of the API as a de facto industry standard and herald the end of its period of rapid fundamental iteration.

From here, we’re going to see a flourishing of support for the Twitter API across the web, meaning that the Twitter API is finished. Not kaput, *complete*. If two companies with a significant number of users that share no investors or board members both support a common API, we can say that the API has reached Version 1.0 and is safe to base your work on. So now what?### How We Got Here

Like a lot of folks, I’ve been thinking out loud and pondering the future of Twitter and open web APIs pretty much all year. Some key ideas have bubbled up:

[The Pushbutton Web](http://dashes.com/anil/2009/07/the-pushbutton-web-realtime-becomes-real.html):

> [A]ny site or application can deliver realtime messages to a web-scale audience, using free and open technologies at low cost and without relying on any single company like Twitter or Facebook.

[The Web Way vs. The Wave Way](http://dashes.com/anil/2009/08/what-works-the-web-way-vs-the-wave-way.html)

> - Upgrades to the web are incremental.
> - Understanding new tech needs to be a weekend-sized problem.
> - There has to be value before everybody has upgraded.
> - You have to be able to understand and explain it.

Those posts from this summer show that the ideas behind the Twitter API’s “overnight” ubiquity have been kicking around in developer circles for months, if not more than a year. Finally, though, we have shipping examples of broad adoption of an API that’s lightweight and suitable for today’s most interesting applications. It’s not just that Twitter’s realtime, though of course that is compelling, but also that these APIs are simple enough for weekend hackers to build interesting projects on, and that they’re easy to implement even on mobile devices and in almost any programming language.

So, today, we have support for the Twitter API from Twitter (of course), WordPress and Tumblr. I know I saw folks working on this for TypePad’s free service when I was at Six Apart, so I’d assume they just wanted to finish OAuth support before supporting it as well. (See below.)

Of course, I don’t need to make any suggestions to developers about what to do with these APIs — I’m sure the gears in everybody’s heads are turning about cool new applications to build. Instead, I’d like to make a series of suggestions for the entire Open Twitter API ecosystem, based on what we’ve learned from past successes and failures in APIs around blogging.

### What Server Developers Should Do

- **Please please please support OAuth**: It’s egregious that the newest implementations of the Twitter API are stil encouraging people to share their passwords with third-party sites. Five or ten years ago, this was common practice in APIs because we didn’t have better options. Twitter started out using shared passwords, but mercifully has started to bring OAuth support online. But for *new* services to be encouraging the horrible practice of users entering their passwords into every application willy-nilly is just unacceptable. I think we have a two-week window or so within which the new services supporting the Twitter API could announce their intention to support OAuth and really catalyze client developers into doing the wrong thing, but I fear we may lose another generation of API evolution to this terrible practice. If just one or two services announce intent around OAuth by the end of the year, client developers will follow — if you use WordPress or Tumblr, encourage your service provider to do this. (This is usually where I’d insert a dozen examples of how sharing passwords screws users, services, and the ecosystem, but I know that developers often just use shared passwords because they’re lazy. Do the right thing, guys. The client devs will follow along.)
- **Support Really Simple Discovery**: [The RSD format](http://en.wikipedia.org/wiki/Really_Simple_Discovery) isn’t sexy by today’s standards, but grew organically out of some smart thinking from when blogging APIs were at the same state of maturity as today’s tweeting APIs. Instead of reinventing the wheel, developers should look at supporting RSD and looking for something like a “tweetsapi” endpoint for these new services. That way, any arbitrary site can advertise that it supports the Twitter API, or even future versions of an open MetaTweets API. Pay attention to which APIs are listed as “preferred”.
- **Think about overloading of `source`**: The `source` element of status updates in the Twitter API is very interestingly open-ended, and supports use of URLs. Instead of merely advertising your client app, smart use of `rel` attributes and URLs here could help bootstrap some very interesting new potential.

### What Client Developers Should Do

- **Support RSD**: Same logic as above.
- **Start sharing parsing libraries**: Client devs going to be doing a lot of duplicate work to parse out URLs and usernames and hashtags and maybe even [slashtags](http://microsyntax.pbworks.com/Slashtags). But almost every scripting language supports some similar variation on regular expressions, and if you’re using that method to tease out meaning from short messages, then lighten your burden by sharing the load. John Gruber’s work to [share his URL parsing rules](http://daringfireball.net/2009/11/liberal_regex_for_matching_urls) should be a model for a dozen other GitHub projects — compete on features and execution, but not on these fundamental interpretations of text.
- **Build in the big services, but support the little ones**: You’ll naturally want to offer menu options for users of the big, centralized hosted services. But (perhaps as part of supporting RSD), you should allow for all of us to have arbitrary Twitter API endpoints on our own domain names — this is good for the web!

### What Every Developer Should Do

- **Think about piping Twitter API endpoints together**: I think it will be common for some kinds of applications that support the Twitter API to be both clients *and* servers, supporting piping content through, and perhaps applying transformations to the updates. This idea of daisy-chaining services together is likely only going to happen if a lot of parts of the infrastructure support OAuth well, but has the potential to be truly revolutionary if the ecosystem allows it to happen.
- **Start looking at people’s firehoses**: Twitter’s firehose of all status updates is about to be broadly available for developers, I know about the free [TypePad firehose](http://www.sixapart.com/labs/update/) from my time at Six Apart, and I think [WordPress will sell you access](http://en.wordpress.com/firehose/) to theirs, but I haven’t yet been able to find a reference for one for Tumblr. No matter — we should assume that free, open versions of these are coming, and start to figure out how to encourage similar collaboration around the reading side of things, now that the writing side of things is getting hashed out.
- **Consider adopting a “+2 Rule”**: The natural inclination right now for geeks of a certain type is to start dreaming up new standards bodies, or how they can participate in the Open Web Foundation to make a Super Awesome Twitter API Evolution Committee. Here’s my recommendation: Don’t. Don’t do any of that shit, and don’t run off to make membership badges for the Treehouse Club quite yet. Instead, just iterate and ship. Keep making new apps and see what you can do to stretch the limits of the existing methods and structures. I love the new geocoding and contributor aspects of the Twitter API, but as I said at the top of this post, I think the period of rapid iteration on the core Twitter API is ending, as new efforts going forward will have to reach consensus.

The good news is, consensus around evolution of the Twitter API can happen simply by saying to each other, “If two application developers who share no common investors or board members can reach agreement around an extension to the API, and between them they have a significant enough number of users to be relevant, then we should all just adopt their work.”

This is important because it reframes the conversation from being about technical merits, and all the boys who like to play with APIs always think they know what’s “better”. I’m sure if I wanted to waste an afternoon, I could tell you a dozen ways in which the Twitter API could be “improved”. But guess what? That shit *does not matter*. Adoption matters, and I’m heartened by the fact that people seem to be getting that.

So, get to work! Please give me feedback if I’m wrong or being stupid about one of my recommendations, but if not, then just start hacking. Stop encouraging people to share passwords, start encouraging services to share tweets, and let’s all join in a hearty session of finger-pointing and mockery in Facebook’s general direction for their sense of Not Invented Here having overshadowed their opportunity, because they could have really clearly done an “embrace and extend (and extinguish)” on the Twitter API if they hadn’t wanted to make their own system a year ago, and now they’ve lost that power.

Finally, thanks a lot to [Dave Winer](http://www.scripting.com/) for essentially inspiring a lot of players in blogging to move towards embracing the Twitter API. Sure, lots of us had the idea, and I’ve spent a lot of times in meetings arguing for this stuff across the industry, and Automattic and Tumblr and others were brave enough to embrace it. But I don’t think anybody’s done more to publicly advocate for an open Twitter API than Dave. I’m glad we’ve evolved as a community to the point where these kinds of breakthroughs aren’t the contentious, immature shitfests they used to be.
