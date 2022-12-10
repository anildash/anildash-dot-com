---
title: Facebook is gaslighting the web. We can fix it.
slug: facebook_is_gaslighting_the_web
date_published: 2011-11-21T17:08:37.000Z
date_updated: 2019-07-23T07:27:26.000Z
tags: Best Of, Most Popular, tech
---

Facebook has moved from merely being a walled garden into openly attacking its users’ ability and willingness to navigate the rest of the web. The evidence that this is true *even for sites which embrace Facebook technologies* is overwhelming, and the net result is that Facebook is gaslighting users into believing that visiting the web is dangerous or threatening.

In this post I intend to not only document the practices which enable this attack, but to also propose a remedy.

### 1. You Cannot Bring Your Content In To Facebook

![Screen-Shot-2011-11-09-at-7.07.42-PM](__GHOST_URL__/content/images/2019/05/Screen-Shot-2011-11-09-at-7.07.42-PM.png)

This warning appeared on Facebook two weeks ago to advise publishers (including this site) that syndicate their content to Facebook Notes via RSS that the capability would be removed starting tomorrow. Facebook’s [proposed remedy](https://www.facebook.com/help/?faq=206051139465982#My-blog-isn't-importing-to-Facebook.) involves either completely recreating one’s content within Facebook’s own Notes feature, or manually creating status updates which link to each post on the original blog. Remember that second option, linking to each post manually — we’ll return to it later.

### 2. Publishers Whose Content Is Captive Are Privileged

Over at CNET, [Molly Wood made a powerful case](http://news.cnet.com/8301-31322_3-57324406-256/how-facebook-is-ruining-sharing) against the proliferation of Facebook apps that enable ongoing, automated sharing of behavior data after only a single approval from a user. In her words:

> Now, it’s tempting to blame your friends for installing or using these apps in the first place, and the publications like the Post that are developing them and insisting you view their stories that way. But don’t be distracted. Facebook is to blame here. These apps and their auto-sharing (and intercepts) are all part of the Open Graph master plan.
> 
> When Facebook unveiled Open Graph at the f8 developer conference this year, it was clear that the goal of the initiative is to quantify just about everything you do on Facebook. All your shares are automatic, and both Facebook and publishers can track them, use them to develop personalization tools, and apply some kind of metric to them.

As Molly’s piece eloquently explains, what Facebook is calling “frictionless” sharing is actually placing an *extremely high barrier* to the sharing of links to sites on the web. Ordinary hyperlinks to the rest of the web are stuck in the lower reaches of a user’s news feed, competing for bottom position on a news feed whose prioritization algorithm is completely opaque. Meanwhile, sites that foolishly and shortsightedly trust all of their content to live within Facebook’s walls are privileged, at the cost of no longer controlling their presence on the web.

### 3. Web sites are deemed unsafe, even if Facebook monitors them

As you’ll notice below, I use Facebook comments on this site, to make it convenient for many people to comment, and to make sure I fully understand the choices they are making as a platform provider. Sometimes I get a handful of comments, but on occasion I see some very active comment threads. When a commenter left a comment on [my post about Readability](http://dashes.com/anil/2011/11/readability-and-intention.html) last week, I got a notification message in the top bar of my Facebook page to let me know. Clicking on that notification yielded this warning message:

![facebook-dashes-warning](__GHOST_URL__/content/images/2019/05/facebook-dashes-warning.png)

What’s remarkable about this warning message is not merely that an ordinary, simple web content page is being presented as a danger to a user. No, it’s far worse:

- Facebook is warning its users about the safety of a page which **incorporates Facebook’s own commenting features**, meaning even web sites that embrace Facebook’s technologies can be marginalized
- Facebook is displaying this warning **despite the fact that Facebook’s own systems have indexed the page** and found that it incorporates their own Open Graph information.

To illustrate this second point, I’ll include what is a fairly nerdy illustration for those interested. If you’re sufficiently interested in the technical side of this, what’s being shown is Facebook’s own URL linter, as viewed through the social plugins area in the developer console for a site. In this view, it verifies not only that the Open Graph meta tags are in place (minus an image placeholder, as the referenced post has no images), but that Facebook has crawled the site and verified enough of the content of the page to know their own comment system is in place on the page. (Click to view the whole page, with only the app ID numbers redacted.)

![FB-open-graph-debug](__GHOST_URL__/content/images/2019/05/FB-open-graph-debug.png)

### How to Address This Attack

Now, we’ve shown that Facebook promotes captive content on its network ahead of content on the web, prohibits users from bringing open content into their network, warns users not to visit web content, and places obstacles in front of visits to web sites even if they’ve embraced Facebook’s technologies and registered in Facebook’s centralized database of sites on the web.

Fortunately, the overwhelming majority of web users visit Facebook through relatively open web browsers. For these users, there is a remedy which could effectively communicate the danger that Facebook represents to their web browsing habits, and it would be available to nearly every user except those using Facebook’s own clients on mobile platforms.

This is the network of services designed to warn users about dangers on the web, one of the most prominent of which is [Stop Badware](http://stopbadware.org/). From that site comes this description:

> Some badware is not malicious in its intent, but still fails to put the user in control. Consider, for example, a browser toolbar that helps you shop online more effectively but neglects to mention that it will send a list of everything you buy online to the company that provides the toolbar.

I believe this description clearly describes Facebook’s behavior, and strongly urge Stop Badware partners such as Google (whose Safe Browsing service is also used by Mozilla and Apple), as well as Microsoft’s similar SmartScreen filter, to warn web users when visiting Facebook. Given that Facebook is consistently misleading users about the nature of web links that they visit and placing barriers to web sites being able to be visited through ordinary web links on their network, this seems an appropriate and necessary remedy for their behavior.

Part of my motivation for recommending this remedy is to demonstrate that our technology industry *is* capable of regulating and balancing itself when individual companies act in ways that are not in the best interest of the public. It is my sincere hope that this is the case.

### Further Reading

Many aspects of this conversation are not, of course, new topics. Some key pieces you may be interested in:

- As I was researching this piece, Marshall Kirkpatrick published [Why Facebook’s Seamless Sharing is Wrong](http://www.readwriteweb.com/archives/why_facebooks_seamless_sharing_is_wrong.php) over on ReadWriteWeb, articulating many of these same concerns. His piece is well worth reading.
- Albert Wenger of Union Square Ventures makes a [strong case](http://continuations.com/post/13109220003/sharing-one-network-to-rule-them-all-or-network-of) for the long-term goal of a network of networks. I fully share his vision here, and hope most in our industry will endorse this idea as well.
- Molly Wood’s [excellent look at Facebook sharing](http://news.cnet.com/8301-31322_3-57324406-256/how-facebook-is-ruining-sharing) which I referenced above is worth reading in its entirety.
- [Blackbird, Rainman, Facebook and the Watery Web](__GHOST_URL__/2007/10/08/rainman_blackbird_facebook_and_the_new_tables/) was a more optimistic look at how web platforms evolve that I wrote four years ago when Facebook was much less dominant.
- [The Facebook Reckoning](__GHOST_URL__/2010/09/13/the_facebook_reckoning-2010/) a year ago offered a perspective on the values and privilege that inform Facebook’s decision-making.
- My ruminations on [ThinkUp and Software With Purpose](http://dashes.com/anil/2011/11/thinkup-1.0.html) last week also explored the related danger of Facebook deleting everything you’ve ever created on their site.
