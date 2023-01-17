---
title: How you could build a search that the fediverse would welcome
slug: a-fediverse-search
date_published: 2023-01-16T20:00:05.000Z
tags: [tech, web, twitter, fediverse]
---

Mastodon and the fediverse are clearly taking off, bringing in millions of new users, and also organically inspiring a wave of technical innovation that dwarfs all of the efforts that the bribes and empty promises of the Web3 crypto bubble couldn't touch. I'm even enjoying having settled into a relatively permanent new fediverse address at <a href="https://me.dm/@anildash">@anildash@me.dm</a>, on Medium's new <a href="https://blog.medium.com/medium-embraces-mastodon-19dcb873eb11">Mastodon instance</a>, which (along with Mozilla's similar <a href="https://blog.mozilla.org/en/mozilla/mozilla-launch-fediverse-instance-social-media-alternative/">upcoming instance</a>) should do a lot ot legitimize the nascent open system. It's all great to see, though of course there are huge challenges that come along with this growth, and most of them (as always, with social media) are largely about people and culture, not technology.

Nothing exemplifies these opportunities and challenges better than search. Search has long been the killer app of the web, since the days of Yahoo and AltaVista on to the long reign of Google's dominance, to today's web where SEO is dying and TikTok is (inexplicably, to text-lovers like me) increasingly on the rise. In that complex environment, the intentional absence of substantial search features in the fediverse, especially in the flagship Mastodon experience that defines the nascent fediverse for so many new users, seems inexplicable. But search is also a signifier to those who pioneered and established the current era of the fediverse, symbolizing the extractive and exploitative hypergrowth systems that often ruined the positivity and promise of the human web. 

Here's one of the most popular posts I'd ever shared on my first Mastodon account.

<iframe src="https://mastodon.cloud/@anildash/109312103250205663/embed" class="mastodon-embed" style="max-width: 100%; border: 0" width="400" allowfullscreen="allowfullscreen"></iframe>

Given that context, it's no surprise that a less experienced fediverse user, no matter how well-intentioned, might well accidentally antagonize some people while trying to build search features for Mastodon users. I've known Jan Lehnardt online for a long time, and known him to make lots of thoughtful things, but I'd missed his initial introduction of Searchtodon, an attempt at introducing personal search (not a public search engine) for the fediverse that I think a lot of long-time fediverse users could have anticipated would cause some consternation, despite his clear intent to be consensual and considered in his implementation. It's well worth reading his <a href="https://searchtodon.social/Adventures-in-Mastoland.html">detailed retrospective</a> on the reaction to the service.

I realize I've had an idea for how to implement Fediverse search for a long time that I've talked about privately with people but not shared broadly, and it's probably doing a disservice to potential implementors to not share some of my thinking. It also seems like it'd be great to float the idea as a _concept_ rather than an implementation, so that people could react to the idea without the increased emotional urgency of feeling like they have to react to an existing potential threat.

## Why search?

The first question to address when talking about creating a search to serve fediverse users is _why do this in the first place_? A lot of people would argue (to varying degrees of thoughtfulness) that this kind of capability shouldn't exist at all. Eugen Rochko, the lead developer and creator of Mastodon, and de facto administrator of community norms and consent for such features across the entire fediverse, addressed this many years ago in a post that I remember being largely non-controversial at the time.

<iframe src="https://mastodon.social/@Gargron/4947733/embed" class="mastodon-embed" style="max-width: 100%; border: 0" width="400" allowfullscreen="allowfullscreen"></iframe>

But interestingly, even that core assertion would likely be strongly debated in an environment that, six years later, feels even more fraught. So let's lay out some key reasons for why a search capability _might_ be a net positive for the fediverse, explore the arguments against it, and then share the parameters of a potential implementation that could deliver on the positives without triggering the negatives.

First, the benefits of search:

* **Search enables content to be citable and referenceable over time.** The web itself was created as a medium for publishing, and then _linking to_ (citing) those published works, and being able to search for an item vastly increases the odds that it will be cited or discovered later, increasing the ability to build knowledge, and especially allowing good ideas to be found later on even if their creators didn't initially have reach or reputation or social access which allowed their ideas to spread at the time they were published.
* **Search can enable people to document their credentials and authority.** This is most vital for people who are part of vulnerable or marginalized communities, where coming with receipts is a fundamental part of asserting authority in a culture that might otherwise dismiss or diminsh their work.
* **Search enables many kinds of fun and creative expressions.** From a technical perspective, hashtags and other forms of group sharing/discovery are just specific implementations of search. These are foundational for many kinds of play 