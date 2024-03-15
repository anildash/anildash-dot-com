---
title: Where Tumblr Came From
slug: where_tumblr_came_from
date_published: 2013-05-20T16:33:32.000Z
date_updated: 2018-04-21T11:04:27.000Z
image: https://cdn.glitch.global/c4e475b2-a54e-47e0-973c-ed0bd1b46262/tumblr-oct-2007.png?v=1670561542680
tags: [tech, blogs, tumblr]
---

Seven years ago, my wife [Alaina Browne](http://alainabrowne.com/) and I were living happily in San Francisco when she went off to NYC to visit with our friends and attend a party. By the time she flew back, we were on a path that not only led to our return to New York City, but to getting a front-row seat to the birth of what would become [Tumblr](http://tumblr.com/). Along the way, I’ve had the chance to see Tumblr from the perspective of a user, a competitor and a fan. Since so much of the conversation today is about the dollar amount of their sale, and the speculation about their future with Yahoo, I thought it’d be nice to look back at a few distinct moments in their evolution, as seen by an interested outsider.

## Before the Beginning

Alaina had come back excited from visiting New York, telling me about having been introduced to [Ed Levine](http://www.seriouseats.com/about-ed-levine/) by our friends [David Jacobs](http://hello.typepad.com/) and [Meg Hourihan](http://megnut.com/). Ed wanted to build a food community site called [Serious Eats](http://seriouseats.com/), and had hired two young guys recommended by [Fred Seibert](http://fredseibert.com/) to build out the site. I heard secondhand from my friends about the content management system that was being built by [Davidville](http://www.davidville.com/), the consulting company run by David Karp and Marco Arment. David and Marco were building a tool to power Serious Eats, but I didn’t know anything about them except that they were really young.

Serious Eats had gotten a launch sponsorship, and as a result needed to get up and running by the holiday season. But by October, all that I’d seen of the publishing tool they were building was a very simple single-column blog that presented photos really nicely, but had no way to show standard banner ads at all. After debating whether the ads that needed to be delivered could be fit into the simple structure of the tool that had been built, the team decided in favor of just launching Serious Eats on off-the-shelf technology because they needed to get running quickly. As [David Jacobs described](http://hello.typepad.com/hello/2013/05/frequently-asked-questions-about-yahoos-acquisition-of-tumblr.html) in his post on the Yahoo/Tumblr deal, the team picked Movable Type since they were all very familiar with the software and knew those of us who worked on making that app.

In short, some of the fundamental constraints that shaped Tumblr in its most nascent stages was that publishers weren’t yet able to get advertisers to buy native, in-stream ad units, and that traditional ad buys made units that were not easy to integrate into super-simple tumblelogs. Hmm!

**Update:** I think Marco had some objections to my characterization of this point in the evolution of their work. His tweets on the matter follow:

> As usual, Anil Dash is wrong: [http://t.co/myos3U6Lxe](http://t.co/myos3U6Lxe)
> 
> Serious Eats and Tumblr shared no code except our generic PHP MVC framework.
> &mdash; Marco Arment (@marcoarment) [May 20, 2013](https://twitter.com/marcoarment/status/336574214805008385?ref_src=twsrc%5Etfw)

> What we built for Serious Eats wasn’t too simple — it was too complex and overreaching.
> 
> It wasn’t a single-column blog for photos… at all.
> &mdash; Marco Arment (@marcoarment) [May 20, 2013](https://twitter.com/marcoarment/status/336576028313014272?ref_src=twsrc%5Etfw)

Given that I made no assertion over how much code was shared between the two companies, and since a simple CMS is usually little more than a nice wrapper around an MVC framework, it seems there’s little in dispute here except whether the content management system was a poor fit for being too complicated or for yielding output that was too simple. I’m happy to believe Marco has a better memory of the project than I do, since he worked on it and I barely even visited.

Marco also offered some other snarking at Meg about whether the client or consultant was to blame for an underspecified set of goals for the content management system, but these things are almost always everybody’s fault, and that’s sort of beside the point which is that the ideas of Tumblr were in tension with conventional blogging of the era.

## Tumblelogs Take Off

Meanwhile, David and Marco took that simple publishing system they’d built and kept refining it. They were insistent even in those early days on calling the output “tumblelogs” instead of just “blogs”, which I mentally filed away as “those sites like [projectionist](http://project.ioni.st/)“.

![tumblr-2007-screenshot](https://cdn.glitch.global/c4e475b2-a54e-47e0-973c-ed0bd1b46262/tumblr-2007-screenshot.png?v=1670561377107 "Screenshot of Tumblr in 2007")

At the time, Tumblelogs had been around for a little while, best known to us old-time bloggers due to Jason Kottke’s [seminal post on Tumblelogs](http://kottke.org/05/10/tumblelogs), which defined the format just as it was about to take off, and featured project.ioni.st as its leading light. But in a classic case of geeks looking at a thing from a technical standpoint instead of from a cultural one, many of us who were familiar with blogs already saw tumblelogs as “just a simple blogging template”, similar to what we were already doing on Movable Type or WordPress at the time, rather than a fundamentally different medium.

Despite that myopia, there was a lot of momentum around simplified, media-rich blogging at that moment in history. Twitter had launched just a few months earlier in mid-2006, without any of its current photo or video capabilities, but with a super-simple posting experience similar to what made Tumblr so easy to use. Much of the early team behind Movable Type had moved to working on a platform called [Vox](http://en.wikipedia.org/wiki/Vox_(blogging_platform)), which was a simpler blogging tool for sharing media from other services, but included privacy features similar to the Flickr or LiveJournal, which kept it from being as dead-simple to use as Tumblr. WordPress, too, had incorporated a feature called “Asides”, based on a popular plugin from Matt Mullenweg, and it made regular posts of photos, quotes and video clips easy to integrate into a more traditional blog.

At a technical level, many of these efforts were descended from a super-geeky concept that folks had been kicking around a few years earlier, called [structured blogging](http://readwrite.com/2005/12/13/structured_blog). The technical focus of people in the community resulted in it having the super-nerdy name “structured blogging” and yielded a set of poorly-adopted technical specifications rather than a usable experience for normal people. But the fundamental idea behind structured blogging was that people would want to easily post the cool stuff they were finding on other sites and publishing in other media such as photo or video. And Tumblr proved that the idea of this kind of sharing was exactly right, even if the “structured blogging” name and implementation was exactly wrong.

One of the most important justifications for putting “structure” around different kinds of content was so they could be aggregated together into a reader, something like Google Reader, or earlier tools like Bloglines or My Yahoo or Userland Radio. The difference with Tumblr was that David and Marco very early on built in their reader, just like Twitter and LiveJournal had done, making viewing and creating take place in almost the same environment, and forming better connections between users on the site.

## Tussling With Tumblr

By the time Tumblr opened up to the public just a few months later, it was clear they’d hit a perfect mix of features to connect with an audience that cared more about expression than technology. [Gina Trapani](http://lifehacker.com/244915/geek-to-live--instant-no+overhead-blog-with-tumblr) was one of the early, enthusiastic users, and as [Marco rightly pointed out](http://www.muleradio.net/newdisruptors/20/) in a podcast the other day, part of what made Tumblr so popular early on was that they let people use their own domain name, with a beautiful design, for free. Other free tools were either more complicated, or like WordPress or Blogger, they charged extra to use a domain name and/or constrained the template customization that a user could do.

Since I worked at the time for a company that mostly made its money by selling paid software and support for blogging, I didn’t really see Tumblr as a threat so much as an interesting new entrant that offered the best free product for many users. I jokingly made a reference to Tumblr a year later on a promo page for TypePad, which I worked on at the time and after [Fred Wilson](http://fredwilson.vc/post/60278304/heres-the-thing-your-tumblr-while-clever-will) and [Bijan Sabet](http://bijansabet.com/post/60289645/heres-the-thing-your-tumblr-while-clever-will) picked it up, [Marco took offense](http://www.marco.org/2008/11/18/heres-the-thing-your-tumblr-while-clever-will), to my great surprise. In retrospect, it was obvious that Marco would see us as competitors and my joke as disrespect, but at the time I really had thought it was clear I was being playful but respectful because Tumblr had made something cool and I had met, and liked the founders.

## Elbow to Elbow

[![Goodbye, 419](http://farm2.staticflickr.com/1002/5180057331_778f0bf336_z.jpg)](http://www.flickr.com/photos/marcoarment/5180057331/)

When I say that I knew Marco and David a little bit, it’s impossible to overstate how close the NYC tech community was at this point. The office where Tumblr was still based back then was 419 Park Avenue South, and Tumblr shared the space with Serious Eats, Next New Networks (now YouTube Next Lab) and Frederator, Fred Seibert’s studio.

When I ran into David around that time a few blocks away at Shake Shack, I excitedly pulled him aside and said “I really think Tumblr is like LiveJournal 2.0”, which is another one of those endorsements that probably sounded to him like a slight or an insult or some willfully obscure reference, but to me was about as high a form of praise as I could offer — LiveJournal is and was the most seminal social networking platform that’s ever existed, and almost nobody had captured the addictive, expressive environment of its friends list as well as Tumblr’s dashboard did.

Part of what I learned in my very-limited interactions with David and Marco in those early days was how disconnected and arrogant my own view of blogging and social software could be. Because Tumblr recapitulated many earlier ideas, albeit in a vastly superior way, I had thought it wasn’t *really* as new as it has turned out to be. And some of this is just generational; My very first impression of meeting the then-20-year-old David and 24-year-old Marco was “Wow, these guys have a really good eye, and are really full of themselves.” I still think both those things are true, and that those traits have served them very well.

But there was also a half-generational gap between me and these millennials, a cultural difference I hadn’t yet understood or reckoned with. It led me (and many others I know) to underestimate what Tumblr’s importance was, and actually retroactively made my analogy to LiveJournal seem more apt than perhaps I’d intended.

## What’s Next

In the case of LiveJournal, I got to watch first hand as many of the most fundamental parts of social networking and blogging were invented and then mishandled as advertising was introduced. But I never thought those mistakes were intrinsic to this kind of evolution in communities – it just required leadership that understood and truly respected a community.

In the case of Yahoo’s acquisition of Tumblr, I mostly don’t have a lot to say — my [Activate](http://activate.com/) cofounder Michael Wolf is on the board and we’ve done work that makes me far from objective in this regard, but even if we hadn’t, I’d be optimistic about this deal. For me, it’s the concepts I wrote about in [Stop Publishing Web Pages](/2012/08/14/stop_publishing_web_pages/) — we’ve found a model for user interaction and social connection that really works, and it feels like the more places that’s adopted and embraced, the better. Whether that’s on Yahoo’s homepage or Tumblr’s Dashboard, or in some new app on my iPhone, we’re reaching a consensus around how we want to connect with each other.

It’s been fascinating to watch Tumblr evolve, and as a member of the New York tech community, I am thrilled for the whole team (and its inestimable investors) on the success of the company. As a blogger, it’s still a really sweet moment to watch the medium of blogging be validated in this way, since a huge number of dollars is a clear signal even to those who don’t understand the artistic and expressive importance of blogging. And as someone who still loves hacking on these kinds of software, it’s been tremendously useful to see my own assumptions and preconceptions be challenged by a new generation of young entrepreneurs and creators who take this medium I’ve watched since its inception, and push it to fascinating and inspiring new forms.
