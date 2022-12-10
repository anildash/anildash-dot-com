---
title: The Missing Building Blocks of the Web
slug: he-missing-building-blocks-of-the-web
date_published: 2018-03-22T21:00:00.000Z
date_updated: 2021-08-02T03:46:46.000Z
heroimage: https://cdn.glitch.global/c4e475b2-a54e-47e0-973c-ed0bd1b46262/building-blocks-berries-01.jpeg?v=1669625487351
tags: [tech, web, html, blogs]
---

At a time when millions are losing trust in the the web’s biggest sites, it’s worth revisiting the idea that the web was supposed to be made out of countless little sites. Here’s a look at the neglected technologies that were supposed to make it possible.

Though the world wide web has been around for more than a quarter century, people have been theorizing about hypertext and linked documents and a global network of apps for at least 75 years, and perhaps longer. And while some of those ideas are now obsolete, or were hopelessly academic as concepts, or seem incredibly obvious in a world where we’re all on the web every day, the time is perfect to revisit a few of the overlooked gems from past eras. Perhaps modern versions of these concepts could be what helps us rebuild the web into something that has the potential, excitement, and openness that got so many of us excited about it in the first place.

[*An aside: Our team at [Glitch](https://glitch.com/) has been hard at work on delivering many of the core ideas discussed in this piece, including new approaches to [View Source](https://medium.com/glitch/tackling-the-biggest-pain-points-in-web-development-57d64afe19dc), Authoring, [Embedding](https://medium.com/glitch/making-learning-to-code-more-accessible-d802effd52bf), and more. If these ideas resonate with you, we hope you’ll check out Glitch and see how we can bring these abilities back to the web.*]

## View Source

For the first few years of the web, the fundamental way that people learned to build web pages was by using the “View Source” feature in their web browser. You would point your mouse at a menu that said something like “View Source” (nobody was browsing the web on a touchscreen back then) and suddenly you’d see the HTML code that made up the page you were looking at. If you squinted, you could see the text you’d been reading, and wrapped around it was a fairly comprehensible set of tags — you know, that `<p>paragraph</p>` kind of stuff.

It was one of the most effective technology teaching tools ever created. And no surprise, since the web was *invented* for the purpose of sharing knowledge.

These days, View Source is in bad shape. Most mobile devices don’t support the feature at all. And even on the desktop, the feature gets buried away, or hidden unless you enable special developer settings. It’s especially egregious because the *tools* for working with HTML in a browser are better than ever. Developers have basically given ordinary desktop web browsers the potential to be smart, powerful tools for creating web pages.

But that leads to the other problem. Most complicated web pages these days aren’t actually *written* by anyone. They’re assembled, by little programs that take the instructions made by a coder, and then translate those instructions into the actual HTML (and CSS, and JavaScript, and images, and everything else) that goes to your browser. If you’re an expert, maybe you can figure out what tools were being used to assemble the page, and go to GitHub and find some version of those tools to try out. But it’s the difference between learning to cook by looking over someone’s shoulder or being told where a restaurant bought its ingredients.

Bringing View Source back could empower a new generation of creators to see the web as something they *make*, not just a place where big companies put up sites that we all dump our personal data into.

![Building Blocks berries](https://cdn.glitch.global/c4e475b2-a54e-47e0-973c-ed0bd1b46262/building-blocks-berries-04.jpeg?v=1669625486996)

## Authoring

When Tim Berners-Lee invented the world wide web, he assumed that, just like in earlier hypertext systems, every web browser would be able to write web pages just as easily as it read them. In fact, that early belief led many who pioneered the web to assume that the format of HTML itself didn’t matter that much, as many different browsing tools would be able to create it.

In some ways, that’s true — billions of people make things on the web all the time. Only they don’t know they’re making HTML, because Facebook (or Instagram, or whatever other app they’re using) generates it for them.

Interestingly, it’s one of Facebook’s board members that helped cause this schism between reading and writing on the web. Marc Andreessen pioneered the early Mosaic web browser, and then famously went on to spearhead Netscape, the first broadly-available commercial web browser. But Netscape wasn’t made as a publicly-funded research project at a state university — it was a hot startup company backed by a lot of venture capital investment.

It’s no surprise, then, that the ability to *create* web pages was reserved for Netscape Gold, the paid version of that first broadly consumer-oriented web browser. Reading things on the web would be free, sure. But creating things on the web? We’d pay venture-backed startup tech companies for the ability to do that, and they’d mediate it for us.

Notwithstanding Facebook’s current dominance, there are still a lot of ways to publish actual websites instead of just dumping little bits of content into the giant social network. There are all kinds of “site building” tools that let you pick a template and publish. Professionals have authoring tools or content management systems for maintaining big, serious websites. But these days, there are very few tools you could just use on your computer (or your tablet, or your phone) to create a web page or web site from scratch.

All that could change quickly, though—the barriers are lower than ever to reclaiming the creative capability that the web was supposed to have right from its birth.

![Building Blocks berries](https://cdn.glitch.global/c4e475b2-a54e-47e0-973c-ed0bd1b46262/building-blocks-berries-03.jpeg?v=1669625486626)

## Embedding (Transclusion!)

Okay, this one’s nerdy. But I’m just gonna put it out there: You’re supposed to be able to include other websites (or parts of other websites) in your web pages. Sure, we can do some of that — you’ve seen plenty of YouTube videos embedded inside articles that you’ve read, and as media sites pivot to video, that’s only gotten more commonplace.

But you almost *never* see a little functional part of one website embedded in another. Old-timers might remember when Flash ruled the web, and people made simple games or interactive art pieces that would then get shared on blogs or other media sites. Except for the occasional SoundCloud song on someone’s Tumblr, it’s a grim landscape for anyone that can imagine a web where bits and pieces of different sites are combined together like Legos.

Most of the time, we talk about this functionality as “embedding” a widget from one site into another. There was even a brief fad during the heyday of blogs more than a decade ago where people started entire companies around the idea of making “widgets” that would get shared on blogs or even on company websites. These days that capability is mostly used to put a Google Map onto a company’s site so you can find their nearest location.

Those old hypertext theory people had broader ambitions, though. They thought we might someday be able to pull live, updated pieces of other sites into our own websites, mixing and matching data or even whole apps as needed. This ability to include part of one web page into another was called “transclusion”, and it’s remained a bit of a holy grail for decades.

There’s no reason that this can’t be done today, especially since the way we build web pages in the modern era often involves generating just partial pages or only sending along the data that’s updated on a particular site. If we can address the security and performance concerns of sharing data this way, we could address one of the biggest unfulfilled promises of the web.

![Building Blocks berries](https://cdn.glitch.global/c4e475b2-a54e-47e0-973c-ed0bd1b46262/building-blocks-berries-02.jpeg?v=1669625486272)

## Your own website at your own address

This one is so obvious, but we seem to have forgotten all about it: The web was designed so that everybody was supposed to have their own website, at its own address. Of course, things got complicated early on — it was too hard to run your own website (let alone your own web server!) and the relative scarcity of domain names made them expensive and a pain for everybody to buy.

If you just wanted to share some ideas, or talk to your friends, or do your work, managing all that hassle became too much trouble, and pretty soon a big, expensive industry of web consultants sprung up to handle the needs of anybody who still actually wanted their own website—and had the money to pay for it.

But things have gotten much easier. There are plenty of tools for easily building a website now, and many of them are free. And while companies still usually have a website of their own, an individual having a substantial website (not just a one-page placeholder) is pretty unusual these days unless they’re a Social Media Expert or somebody with a book to sell.

There’s no reason it has to be that way, though. There are no technical barriers for why we couldn’t share our photos to our own sites instead of to Instagram, or why we couldn’t post stupid memes to our own web address instead of on Facebook or Reddit. There are social barriers, of course — if we stubbornly used our own websites right now, none of our family or friends would see our stuff. Yet there’s been a dogged community of web nerds working on that problem for a decade or two, trying to see if they can get the ease or convenience of sharing on Facebook or Twitter or Instagram to work across a distributed network where everyone has their own websites.

Now, none of that stuff is simple enough yet. It’s for nerds, or sometimes, it’s for nobody at all. But the same was true of the web itself, for years, when it was young. This time, we know the stakes, and we can imagine the value of having a little piece of the internet that we own ourselves, and have some control over.

It’s not impossible that we could still complete the unfinished business that’s left over from the web’s earliest days. And I have to imagine it’ll be kind of fun and well worth the effort to at least give it a try.

![Building Blocks berries](https://cdn.glitch.global/c4e475b2-a54e-47e0-973c-ed0bd1b46262/building-blocks-berries-05.jpeg?v=1669625485904)


> In a similar vein, you may also enjoy this look at [the lost infrastructure of the early era of social media](/2016/08/08/the-lost-infrastructure-of-social-media/).
