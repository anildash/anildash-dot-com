---
title: Your Whole Life In One Tweet
slug: one_line_bios
date_published: 2010-10-04T04:48:28.000Z
date_updated: 2021-04-22T20:00:53.000Z
heroimage: https://cdn.glitch.global/c4e475b2-a54e-47e0-973c-ed0bd1b46262/conan-twitter-bio.png?v=1670823760124
tags: [tech, media, software, twitter]
---

There’s an odd tendency in web culture to see all features as obvious, even inevitable. While most of the artifacts of our computing experience have been invented recently, in living memory, we treat them as if they existed centuries ago and that the names of their creators have been lost to history. But the features that pervade the social web were created by people, sometimes not even by teams, but by individual men and women. And because the web itself is so young, these creators are overwhelmingly still alive, still active in creating the web, and working in our midst where we can learn from their lessons.

## Get In Line

For example, take a look at your bio on any given site, it’s usually right there next to your profile picture. Whether it’s Facebook or Twitter or LinkedIn or almost anywhere else, there’s probably a brief description of yourself. These days it’s probably under 140 characters, to meet Twitter’s limits, or under 160 characters, to meet SMS restrictions. But there it is, ubiquitous and omnipresent. Surely, it must have just always have been on the web, right? Like RSS, or the comment form on a web page, or all the other little features we take for granted, it’s one of those things that seems so obvious in retrospect that it’s hard to believe it was created.

[![The lovely David Galbraith...](http://farm1.static.flickr.com/46/118053702_179ebe81f7_m.jpg)](http://www.flickr.com/photos/plasticbag/118053702/)

Except that these short biographies, originally named “One-Line Bio”, *were* created, and even more, they were created by a single guy: [David Galbraith](http://davidgalbraith.org/aboutme/). Now, David’s a friend, so it might seem like I’m just building up the reputation of a friend who’s far too modest (David also helped found Yelp, co-founded early news feed pioneer Moreover, and co-created RSS 1.0, among other things) but I thought exploring the history of this little artifact of web culture might be a good reminder that there are probably thousands of other similar small inventions just waiting to be used by hundreds of millions of people on the web. And David’s also an architect by trade — not a software architect, but a *real* architect, who knows how to judge if something is going to fall down on your head. Perhaps that discipline offers some lessons about what it takes to build structures that have permanence, and that are designed to be inhabited.

In the case of one-line bios, we’re particularly fortunate since, thanks to the Magic Of Blogs™, we can actually see the genesis of this little feature of the web, documented [in David’s archives](http://davidgalbraith.org/category/metadata/).

- [January 13, 2003](http://davidgalbraith.org/metadata/weblogs-and-bios-add-this-tag-and-i-will-put-you-in-my-blogroll/124/): David asks other bloggers to send him one-line descriptions of themselves to be added to his blogroll. This was not an uncommon tactic of testing out new features in blogging back then, though that period in blogging’s evolution was coming to an end and David’s request may have been the last successful one of the kind, coming as it did before blogging software had really become a competitive business.
- [January 14, 2003](http://davidgalbraith.org/metadata/one-line-bios-are-personal-headlines/126/): The next day, David reveals his hand. The name “one-line bio” appears, describing them as personal headlines, and hinting at what he’d like to do with XML by describing them with the tag . Later the same day, David described an XML vocabulary for the new bios (which [still lives on](http://vocab.org/bio/0.1/olb.html)).

## OLB is Born

As it turned out, cramming lots of extra data into RSS feeds didn’t really take off on the public web much, except for including rich media for podcasts. So the work done to express one-line bios in a machine-readable format was largely a dead end. But the idea of the simple description of a person that would appear as part of their profile was almost immediately adopted, showing up as just a simple section on a regular web page. Part of the reason the suggestion succeeded was that David was well-known to all of the major creators of blog software at the time, making a brief post on this blog a surprisingly effective method of propagating a technical proposal.

The first implementation I saw was [Ben Trott](http://ben.stupidfool.org/)‘s work; He built OLB support into (then not-yet-launched) TypePad immediately and within a few months many of the most influential blogs had added similar descriptors. Friendster launched just a few months after David’s post and quickly added similar brief bio lines as well, doubtless influencing all the later social networks that followed.

Since then, the bio system has gone on to become ubiquitous. As with many such tech developments, the constraint that it introduced became one of its greatest strengths, reducing the burden of writing a full biography of oneself into the simple task of writing a one-line bio just as you’d do to introduce yourself at a cocktail party.

That parallel became particularly clear to me when I ran in to David at the [party for Dave Winer](http://www.scripting.com/stories/2010/03/04/lastNightsSohoParty.html) that Nick Denton had thrown earlier this year, just a few days after Conan O’Brien had [joined Twitter](http://twitter.com/#!/conanobrien/status/9596834783). Amidst all of the buzz about Conan having joined Twitter, what I was most struck by was his simple one-line bio: “I had a show. Then I had a different show. Now I have a Twitter account.” Despite being funny, accurate and self-deprecating, it read to me almost like the headline on an obituary — the briefest possible summary of a life’s work.

In that way, one-line bios strike me as offering some important lessons about the architecture of meaningful things on the web: They should be brief, and structured just enough to give you a starting point without constraining your creativity. They should pack in enough meaning that they have value on their own, but be useful when annotating a larger work. They should be portable enough to work on almost any kind of website. And they should be useful enough that they can succeed even if the ego of their creators is modest enough to not demand credit.

Although David, if you *do* want credit, putting “inventor of one-line bios” in your one-line bio might be a good place to start.
