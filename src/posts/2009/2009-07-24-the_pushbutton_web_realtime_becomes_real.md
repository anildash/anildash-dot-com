---
title: "The Pushbutton Web: Realtime Becomes Real"
slug: the_pushbutton_web_realtime_becomes_real
date_published: 2009-07-24T12:34:55.000Z
date_updated: 2009-07-24T12:34:55.000Z
tags: [Best Of, Most Popular, tech, blogs]
heroimage: https://cdn.glitch.global/0702605b-00dd-404e-8996-743dade19acb/pushbutton-delivery.png?v=1671507589941
---

**Pushbutton** is a name for what I believe will be an upgrade for the web, where any site or application can deliver realtime messages to a web-scale audience, using free and open technologies at low cost and without relying on any single company like Twitter or Facebook. The pieces of this platform have just come together to enable a whole set of new features and applications that would have been nearly impossible for an average web developer to build in the past.

## Background

The most interesting area of new development on the web is the innovation happening around realtime messaging, the ability to deliver updates to a website or application in one or two seconds. While various systems like Yahoo News Alerts or feed readers like Google Reader have offered some simple ways of delivering fairly fast notifications, they are still built on an infrastructure that relies upon requesting a web page repeatedly. These systems do the equivalent of hitting the “reload” button in your web browser over and over.

While those systems have been using these inefficient methods to deliver updates, newer platforms like Twitter, Facebook and FriendFeed have focused on building the infrastructure for efficient large-scale delivery of updates using their own proprietary networks. A lot of attention has been paid to Twitter’s 140-character limit, or Facebook’s News Feed, but the compelling technology that enables the user experience on these platforms is the immediacy with which updates are delivered. Earlier systems like instant messaging or chat allowed realtime messaging on a one-to-one or small group basis, but it’s been harder to deliver those realtime messages to anyone in the world who wanted to receive them unless you had a lot of money, expertise and infrastructure.

Another barrier is that, while there are many different programs and clients that let you connect to Twitter or Facebook with your own applications, there haven’t been any free and open options for delivering realtime messages to a large audience if you couldn’t, or didn’t *want to*, rely on those companies.

But recently, a few key pieces have fallen into place that make it inexpensive and relatively easy to add realtime messaging as an incremental upgrade to existing websites and web applications. This set of related technologies, which I’m calling the Pushbutton platform, will yield a broad new set of capabilities for users, publishers and developers on the web. Best of all, **Pushbutton technologies are free, open and decentralized**, meaning that the arrival of realtime on the web will not be owned or controlled by any single company.

## Defining Pushbutton

The concept and potential of Pushbutton is a lot like [Ajax](http://adaptivepath.com/ideas/essays/archives/000385.php) — it’s not a single technology or invention, it’s a whole family of technologies, some of which have been in development or deployment for nearly a decade, that together enable this new realtime web. Pushbutton’s foundation is built on these systems:

- [Atom](http://en.wikipedia.org/wiki/Atom_%28standard%29) and [RSS](http://cyber.law.harvard.edu/rss/rss.html): The most common feed formats, for syndication on the web
- [PubSubHubBub](http://code.google.com/p/pubsubhubbub/) and [RSSCloud](http://rsscloud.org/): Powerful new “hubs” for distributing messages
- [Web Hooks](http://webhooks.pbworks.com/): Simple web services for receiving messages, rather than sending them

Pushbutton systems rely on the web’s fundamental HTTP protocol for communication between these component parts. The architecture of Pushbutton message delivery is also simple to understand. Before Pushbutton, in today’s systems, when you create a message (a blog post, tweet or other update) that’s published in your RSS or Atom feed, every application or site that wants updates from you has to repeatedly request your feed to know when it’s updated. You can optionally notify (“ping”) some applications to tell them it’s time to come collect your new updates, but this is time-consuming and resource-intensive on both sides, especially if you want to notify a lot of people.

In the best case, the system we have now is analogous to a person coming by your house and saying “Hey, there’s a new edition of your favorite newspaper today. You should go get it.” And then you have to go to the newspaper’s printing plant to pick it up. In a Pushbutton web, that person is delivering each story to your house the moment it’s complete.

That’s because Pushbutton-enabled applications will improve upon the current state of affairs by proactively delivering not just the notification that there’s a new message, but the content of the *message itself*. And instead of requiring all those applications to come to your site to read the update, it uses a hub server in the cloud to pass along the message directly to all the receivers that are interested in it.

![pushbutton delivery](https://cdn.glitch.global/0702605b-00dd-404e-8996-743dade19acb/pushbutton-delivery.png?v=1671507589539)

1. You, the Sender, create a message to be delivered via RSS or Atom

2. Your application gives the messsage to one or more PubSubHubBub or RSSCloud hubs, which reside in the Cloud

3. The PubSubHubBub or RSSCloud hubs deliver the message to any Receivers, the applications or sites that have requested updates from you

In this way, each time you create a new message, a large number of Receivers can consume that message in near realtime (usually less than a second) without a lot of complexity. This kind of messaging has been possible with custom-built or more obscure technologies in the past, but the Pushbutton ecosystem is a breakthrough for a few reasons:

- Sending messages just requires a **minor change** to an RSS or Atom feed, and a simple, well-defined update notification, instead of major changes to the application where you create your messages.
- Receiving messages is also **very simple**, only requiring a developer to handle incoming notifications of updates.
- Most of the system’s **complexity is handled in the hub servers**, which are well-documented, implementable in a variety of programming languages, and built around open code that will likely attract a large developer community.
- Most of the scaling effort and expense happens at the hub level, and all current hubs are **designed to run on inexpensive cloud systems** like Google App Engine or Amazon’s EC2.
- The software for Sending, Receiving or running a hub is **free, open source and available** on almost any platform.
- Messages sent on Pushbutton platforms are **delivered via HTTP**, which is familiar to any web developer and runs well on any hosting environment. All requests between the different layers of a Pushbutton system can be made as simple REST calls.
- Pushbutton technologies can be **adopted incrementally**, so that features can be added piecemeal on either the sender or receiver side, without requiring a wholesale upgrade to infrastructure or application architecture.

## Who’s Behind Pushbutton?

Pushbutton technologies have been created and advocated by some of the most credible and experienced developers of social web technologies. Here’s a brief overview of the impressive pedigree of these components:

- PubSubHubBub was co-created by [Brad Fitzpatrick](http://brad.livejournal.com/) and [Brett Slatkin](http://www.google.com/profiles/bslatkin) of Google. Brad was founder of [LiveJournal](http://livejournal.com/), and created or co-created fundamental social web technologies like [Memcached](http://en.wikipedia.org/wiki/Memcached), [OpenID](http://openid.net/) and more.
- [XML-RPC update pings](http://www.weblogs.com/api.html), RSS and the RSS Cloud ideas were pioneered by [Dave Winer](http://scripting.com/), who has been actively developing open implementations of each of these technologies.
- Web Hooks have been evangelized by [Jeff Lindsay](http://progrium.com/), and have been deployed by a variety of different companies and platforms which all independently developed the technique.

In addition, Google has supported Brad and Brett’s development of PubSubHubBub, and enabled it on the Google FeedBurner service. A number of smaller companies are deploying large parts of this infrastructure as well. In short, some of the best reputations in developing open web systems have made Pushbutton possible, from the biggest tech companies to the most steadfastly independent developers on the web.

## Related Ideas and Prior Art

There are a lot of existing technologies that have influenced the creation and evolution of Pushbutton technologies; If you’re familiar with any of these systems, you’re probably already ahead of the curve in understanding part of what Pushbutton is trying to enable.

- Twitter [Firehose](http://apiwiki.twitter.com/Streaming-API-Documentation), FriendFeed [SUP](http://code.google.com/p/simpleupdateprotocol/), TypePad [Update Stream](http://www.sixapart.com/labs/update/): These realtime delivery systems offer up the content of their respective platforms as an unending stream that developers can consume and use in their applications. At the present time, they all have varying licenses and degrees of openness, and slightly different formats for delivering updates, but have proven the utility of the “sending” part of Pushbutton’s realtime functionality.
- [XMPP](http://xmpp.org/about/) (Jabber), [NNTP](http://en.wikipedia.org/wiki/Network_News_Transfer_Protocol) (Usenet), [IRC](http://en.wikipedia.org/wiki/Internet_Relay_Chat): These older internet protocols all delivered various degrees of realtime messaging and distributed messaging capabilities, and can form a very useful base of experience for Pushbutton developers to learn from. In some cases, fundamental architectural choices about security, authentication or architecture were made when the Internet was less populated and less complex, making them inappropriate for today’s applications. In all cases, these protocols are less-known by most contemporary web developers, and thus lack familiar toolkits and development resources, which make them quite challenging to deploy in common, inexpensive environments.
- [TrackBack](http://en.wikipedia.org/wiki/Trackback) and [Pingback](http://www.hixie.ch/specs/pingback/pingback): These systems for delivering updates between blogging systems were very effective in enabling rich distributed conversations in the early days of the blogosphere. These have declined in usefulness due to poor or missing implementations of authentication, which led to spam problems, and a general lack of understanding of their utility by a lot of newer bloggers. Pushbutton may offer an opportunity to restore some of the value of the idea behind these systems.
- [Reverse HTTP](http://www.reversehttp.net/) may end up being a useful component of some Pushbutton deployments, as a complement or companion to [Comet](http://en.wikipedia.org/wiki/Comet_%28programming%29) and [related](http://en.wikipedia.org/wiki/Comet_%28programming%29#Alternatives) techniques.

## What should we worry about?

- **A format war?** If you’re familiar with the communities around technologies like feeds, you may know they have a deserved reputation for being contentious and even breaking into heated disputes over arcane details. I don’t think that’s likely to happen this time, because there are only one or two viable formats for each layer of the platform, and the creators of each part have shown some consistent good-faith efforts to promote interoperability where possible and peaceful coexistence where necessary. In the Ajax community, for example, the “X” in Ajax often stands for JSON instead of XML, but this hasn’t hindered its broad adoption at all. I’m also willing to personally commit to try to prevent any kind of interpersonal conflict that would inhibit the adoption of Pushbutton technologies. Worry? **No.**
- **Scaling issues?** There will inevitably be some learning to do about how to scale the resource-intensive hub layer of a Pushbutton system. But because the hubs live on cloud systems that make enormous amounts of computing resources easily available, because the coders creating the reference implementations of the hub software have great experience making web-scale systems, and because it’s relatively simple to introduce new hubs as needed, this will likely not be a gating factor for adoption of Pushbutton. Worry? **No.**
- **Intellectual Property Concerns?** I’m not a lawyer, and this isn’t legal advice. But there has already been a great deal of interest in these systems, and it’s likely that any bad actors who were interested in throwing their patent lawyers at this sort of system would probably already be suing people left and right. And the main players who are already involved have shown a consistent desire to make truly open systems that don’t have IP encumbrances. Put simply, I think anybody smart enough to invent these kinds of technologies is smart enough to not want to look like jerks by suing somebody for using them. Worry? **Probably not.**
- **Competition from centralized systems?** Pushbutton technologies are not just free and open, they’re decentralized, which is a serious threat to the “[lobster trap](http://news.gilbert.org/OutsmartingFacebook)” model of social software. We can expect serious competition from the centralized networks that are currently building these sorts of systems. If a threat arises to Pushbutton’s adoption, this is the most likely source. Worry? **Definitely.**
- **Bad user experience?** One of the worst things we can do in making use of new technologies is to ignore the social, personal or even political implications of their use. Messages that are immediately delivered can’t, by their nature, be erased from all the places they appear. The idea of permanently archiving these types of messages is unfamiliar to a lot of less technically-savvy users. And whenever we see something shiny and new, we have the temptation to use technology for technology’s sake, whether or not we’re solving a real problem or providing a real value. If Pushbutton gets a bad rap early on despite having tremendous potential, this will be why. Worry? **Hell, yes.**

## Conclusion

I have tremendous excitement about the new realtime era of web applications. While I’m fundamentally an optimistic person, I have great skepticism when it comes to mindless hype about new technologies, so it’s with a bit of reluctance that I indulge in some hype myself. But I think the Pushbutton web has the opportunity to give individuals and organizations with distinct and passionate voices the ability to be even more immediate and expressive on the web, and [after ten years](/2009/07/20/ten_years.html) of publishing on the web, that’s the part I love the most.

![Wired's notorious 1997 "Push" cover](https://cdn.glitch.global/0702605b-00dd-404e-8996-743dade19acb/wired-push.jpg?v=1671507816907)

I have no doubt that some skeptics will say “Pushbutton is just PubSubHubBub by another name”, just like they said “Ajax is XMLHttpRequest by another name”, and if that’s what the super-geeky guys want to believe, I’m fine with that. And I’m sure there will still be some significant technical details to resolve. But I think by giving the overall concept an approachable, understandable name and (hopefully!) an explanation that can be understood by anyone with an interest, it can catalyze interest in a whole new area of innovation on the web. And to be honest, when I see folks like Brad Fitzpatrick and Dave Winer hacking on the same set of problems, I can’t help but think something interesting will come of it.

Over the next few days, I’ll be outlining some of the opportunities around Pushbutton, espousing more of the philosophy that has the potential to imbue Pushbutton with a bit more meaning than most new web tech, and providing some simple explanations of how you can get started both learning about and taking advantage of these technologies. Most of all, I hope you’ll offer your pointed criticisms, thoughtful critiques, detailed corrections and even better ideas. I’ll be following the conversation here in the comments, across the blogosphere, and on Twitter using the tag #[pshb](http://search.twitter.com/search?q=pshb).
