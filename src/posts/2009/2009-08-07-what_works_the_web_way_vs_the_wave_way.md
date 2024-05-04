---
title: "What Works: The Web Way vs. The Wave Way"
slug: what_works_the_web_way_vs_the_wave_way
date_published: 2009-08-07T17:30:24.000Z
date_updated: 2019-11-14T05:39:06.000Z
tags: [Best Of, Most Popular, tech]
---

Google Wave is an impressive set of technologies, the kind of stunningly slick application that literally makes developers [stand up and cheer](http://smarterware.org/1955/the-google-wave-highlight-reel). I’ve played with the Google Wave test sandbox a bit, and while it’s definitely too complex to live up to the “this will replace email!” hype that greeted its launch, it certainly has some cool features. So the big question is whether Wave will succeed as overall in becoming a popular standard for communications on the web, because Google has made an admirable investment in documenting the underlying platform and making it open enough for others to build on and extend. I think the answer is no, and the reason is because the Wave way is not compatible with the Web way.

What do I mean by “the Web way”? Well, if we look at the history of new technologies being adopted to extend web sites and enhance communications, we see a few trends emerge:

- **Upgrades to the web are incremental.** Instead of requiring a complete overhaul of your technical infrastructure, or radical changes to existing behaviors, the web tech that wins is usually the sort of thing that can be adopted piecemeal, integrated as needed or as a normal part of updating one’s websites or applications.
- **Understanding new tech needs to be a weekend-sized problem.** For a lot of web developers, long before they start integrating a new protocol or platform into their work, they hack together a rough demo over a long weekend to make sure they truly grasp how it works. And a weekend-scale implementation on a personal site usually translates roughly into a 90-day implementation cycle in a business context, which is a reasonably approachable project size. (In tech, three days in personal effort often translates to three months of corporate effort.)
- **There has to be value *before* everybody has upgraded.** This is basically a corollary to [Metcalfe’s Law](http://en.wikipedia.org/wiki/Metcalfe's_law). While we know networks increase in value as they add more nodes, the nature of web tech is that, in order to be worthwhile, it has to provide value even if the people on the other end haven’t upgraded their software or web browsers or clients or servers. Otherwise you’re shouting into an empty room.
- **You have to be able to understand and explain it.** Duh.

Now, if we take a look at some examples of what *has* worked, we can see how various successful technologies have displayed these traits. One great example is feeds. When RSS feeds were new, it was easy to understand their potential immediately, and since I was working at a newspaper at the time, I just spent an afternoon understanding the format and hacking together a quick feed of headlines that anybody could subscribe to. If nobody had adopted feedreaders yet, that was no problem, since there was no cost to just having the feed sit there with no subscribers — the “nobody’s upgraded” problem would only result in me having wasted a few hours.

Ajax had a similar adoption pattern. It took a little bit more time to comprehend, but not much more than an afternoon, and the development effort required for adding Ajax enhancements to an application started as a weekend-scale project and has only gone down over time. Following the principles of [progressive enhancement](http://en.wikipedia.org/wiki/Progressive_enhancement), well-designed implementations performed just fine on older browsers or systems that couldn’t handle the new features. And most sites that have added Ajax features have done so by adding the requirements as a checklist item in the course of normal ongoing updates, not as standalone efforts to migrate to a new technology.

![190-google-wave-thumb](__GHOST_URL__/content/images/2019/11/190-google-wave-thumb.jpg)

This brings us to Wave. Wave offers excellent opportunities to extend its core features and to add richness to its “wavelets”, and I have no criticisms over its utility as a developer platform that third parties can build upon. But the fundamental Wave protocols are, I fear, a bit too complex to ever be fully and correctly implemented by anyone other than Google. Interoperability is likely to be a challenge that plagues the platform for its entire existence. In short: It’s likely that nobody will ever build a fully-compatible clone of Wave that competes with Google’s own implementation.

Why is that true? Let’s look at what’s built in to Wave:

- Powerful realtime collaboration features
- Unlimited versioning of content
- Built around robust XMPP protocol
- Combines chat, document editing, and message threading — wikis + blogs + comments + IM
- Delivered as a very polished rich user interface

Each of these is a very compelling experience. But a lot of developers’ reactions to seeing them was not just “I can’t wait to use that!” but also “I want to add that one feature to my own existing application!”. And that’s where it gets tough. Let’s take a look at Joe Gregorio’s list of [the protocols that power Wave](http://bitworking.org/news/431/wave-first-thoughts). (Joe works at Google, but made this list before he was working on Wave. I appreciate his research and openness on this topic, and presenting his work here is a tribute to what makes Wave *great*, not a criticism of his effort.)

- Federation (XMPP)
- The robot protocol (JSONRPC)
- The gadget API (OpenSocial)
- The wave embed API (Javascript)
- The client-server protocol (As defined by GWT)

That’s a lotta stuff! XMPP alone is a bear to implement, let alone to deploy at large scale. (I can’t think of anyone outside of Google, Earthlink and LiveJournal who have deployed XMPP to millions of users.) But if you wanted to make another application that truly interoperates with all that Wave can do, combining all of these pieces would just be the *starting point*.

And people aren’t *looking* for a replacement for email, or instant messaging, or blogs, or wikis. Those tools all work great for their intended purposes, and whatever technology augments them will likely offer a different combination of persistence and immediacy than those systems. Right now, Wave evokes all of them without being its own distinctive thing. Which means it’s most useful in providing reference implementations of particular new features.

If a developer wants one of the compelling individual features of Wave, like near-realtime collaboration, they’re more likely to use something like (wait for it…) [Pushbutton technologies](http://dashes.com/anil/2009/07/the-pushbutton-web-realtime-becomes-real.html). The infrastructure afforded by the components of the Pushbutton Platform comes nowhere near the richness and polish displayed by Google Wave. Pushbutton isn’t even designed to offer the benefits demonstrated by Wave. But to its credit, Pushbutton displays nowhere near the complexity of Wave in its interoperability requirements. More importantly, integrating Pushbutton features into a website or application isn’t a monolithic process of building dozens of cutting-edge features, but rather can be deployed incrementally by even non-expert webmasters.

In this context, it might help to think of Pushbutton tech as a “micro-Wave”. As [Gina Trapani said](http://lifehacker.com/5331165/the-pushbutton-web-now-in-google-reader) in mentioning Google Reader’s support for PubSubHubBub:

> Huh-wha? you ask. Yeah, I know. It’s no Google Wave. But that’s what makes this exciting. This kind of small Pushbutton implementation is how real web pages will easily use existing technology to notify one another of new updates. The Google Reader/FriendFeed integration is just the first tiny step in what will be a broad deployment of realtime-enabled sites. These sites and services will let one another know when they have new data to share without the sucky inefficiencies of polling. Check out how fast FriendFeed updates when you share an item in Google Reader in the video above.

> In short, it’s almost zero latency.

Why is this clearly “inferior” technology going to win? Well, as just one example, XMPP is way too complicated for any normal human to deploy. Whereas if you’re reading this, you probably *already* have access to a regular HTTP web server that could talk to a Pushbutton hub. In fact, the only two backers I know who *have* worked extensively with XMPP are Brad Fitzpatrick and Artur Bergman, who co-created [Djabberd](http://www.danga.com/djabberd/). And they are both excited about PubSubHubBub. Realistically, someone like Yahoo might try to do all of this, and inevitably one or two open source projects will try to lash together open implementations of each of these pieces to make a kind of FrankenWave application. There are probably already one or two teams working on the inevitable “Enterprise Wave Server” platforms as well, though I haven’t heard about them myself. These efforts may succeed, but that doesn’t mean they’ll ever be robust enough that people will trust them for communicating on the web.

More to the point, I’m a regular blogger who knows a little bit about scripting on a normal web server. I can poke around the documentation and add a few tweaks to my RSS feed (or, in my case, do nothing and have Feedburner automatically handle it for me), and all of a sudden my blog’s feed is part of the Pushbutton web, ready for others to build on. I literally wouldn’t even know where to start with the Wave developer documentation if I wanted to integrate it with my site or any of the little apps I like to hack on during a long weekend. What seems more realistic — that someone will figure out a way to incrementally build on top of realtime feeds to enable Wave-like experiences, or that all this talk of [Waves, wavelets and blips](http://code.google.com/apis/wave/guide.html) is going to suddenly become easy to understand.

In short, web-way tech like feeds, Ajax and Pushbutton win because people who make good sites and applications have a place to start with it. Does this mean we get fancy realtime simultaneous editing right away, now that Pushbutton exists? Nope. In fact, Wave might even get the early jump on those kinds of features for web apps, simply because it’s pioneered that part of the user experience. But Wave only runs to its full potential on the most cutting-edge web browsers. And there may only be a dozen companies in the world with the in-house expertise to clone the entire complement of technologies underlying Wave in order to make a full-fledged competitor. Worse, the monolithic nature of the Wave experience means it will even be a challenge to make a full-fledged open source competitor to the official Google service.

I hope that Wave succeeds, because I love to see ambition and innovation rewarded. But I think it’s mostly likely that Wave’s success will be in inspiring people to create similarly compelling experiences by adding incremental enhancements to their existing sites. That’s how the web’s always advanced in the past.

**Related Reading**:

- [The Pushbutton Web: Realtime Becomes Real](http://dashes.com/anil/2009/07/the-pushbutton-web-realtime-becomes-real.html)
- [The Pushbutton Web now in Google Reader](http://smarterware.org/2665/the-pushbutton-web-now-in-google-reader) (from Smarterware)
- [My keynote session on Pushbutton](http://www.web2expo.com/webexny2009/public/schedule/detail/10504), which will be at the upcoming Web 2.0 Expo in New York City.
