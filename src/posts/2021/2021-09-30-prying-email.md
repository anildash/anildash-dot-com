---
title: Burners, Pollution,  Control & Privacy By A Thousand Cuts
slug: prying-email
date_published: 2021-09-30T07:00:42.000Z
date_updated: 2021-09-30T07:00:42.000Z
heroimage: https://cdn.glitch.global/c4e475b2-a54e-47e0-973c-ed0bd1b46262/Alexander%20Andrews-broken-phone.jpeg?v=1669523043836
tags: [tech, software, culture]
---

The key to protecting people's privacy on the internet isn't in trying to stop users' data from being sent to different services, it's in poisoning the well by having user data be so inconsistent, disconnected, spurious or expensive to collect that today's surveillance infrastructures (often referred to as "ad tech" ) get flummoxed when trying to track you. The "wall" metaphor for keeping data in and companies out is the wrong way to think about it; instead you want to go for a "death by a thousand cuts" offense against powerful antagonists like the surveillance platforms, or to use the nicer phrasing of the tech security community, it's "defense in depth". 

Make it complicated and expensive to do creepy things you, without great complexity or expense to yourself.

A perfect example here is email. All of us use email addresses to log into different sites and apps. But what's often not visible is that those sites trade information about us based on our email address, so the site where you buy lava lamps and torchières can tell the site where you buy fire insurance that they should raise your rates.

"But their privacy policy says they don't do that!" you exclaim, since you love to read privacy policies in full. And maybe they *technically* don't sell that data based on your exact email address. Instead, they might attach that tracking record of your purchase history to an obscured version of your email address. It's like a valet parking ticket, it doesnt say "this person owns this car", it just says "you can find this person's car in this space". Then they give out duplicates of your valet ticket to anyone who pays them money, so the fire insurance company can look up your record too. Technically they didn't sell your data attached directly to your email, it's just that anyone else who already has your email address can buy access to the data. And *everyone* has your email address.

For people bought into the surveillance economy, this constitutes "privacy" for you, because all the data aren't in one place and theoretically the insurance website only has your email address by your explicit permission. In reality, this is not part of what normal people think is happening with their info and it creeps them out. All of this is in addition to things that you already know about, like cookie-based tracking, which enables the helpful feature where you look at a pair of shoes once and then it haunts you on every website you visit forever.

For extra fun, sites can *combine* the cookies and the email-based tracking and make a data profile about you that follows you everywhere on the web whether you're logged in or not. It's also possible to infer connections between bits of data that are likely from the same user; in our valet parking analogy, the parking attendant knows that the Tesla belongs to the guy wearing Allbirds without having to see the valet ticket. A lot of the investment going into machine learning and AI is primarily about training data models to recognize patterns and make connections or extrapolations (however imperfect and biased) from large data sets, and now you know why.

So that's one big reason why Facebook can afford to destabilize democracy globally. But let's get back to the death by a thousand cuts.

## Data Pollution

For the first time since the rise of today's dominant social networks, privacy tech is starting to outpace surveillance tech in a few small areas. In the early 2000s, there was a wave of tools called "pop-up blockers" that users could install in web browsers to stop an early, invasive, super annoying form of display advertising. This didn't do much to stop data *tracking* (Google's ad platform was still nascent then, and most people ignored the warnings about the coming age of data surveillance) but it at least set a precedent for some user control over ads.

In a modern context, we now have fairly robust ad blockers that are much more aggressive about stopping ads, broad limitations on cookie tracking that are supported by both web browser settings and regulation (not to mention the ubiquitous and futile "I accept this cookie" alerts littering the web), and the newest area of great innovation — email protections.

Many services let you create "burner" email accounts, disposable single-use addresses that a site can't track back to your real address. When a message is sent to the burner address, it gets forwarded to your real inbox, and the whole thing is invisible to the site that you're using. (In the old days, those of us who own our own domain names would use one off-addresses for each services to accomplish the same thing, like if I signed up for Amazon with amazon@example.com but used apple@example.com to log in to the App Store.)

Apple built a version of these burner emails right into their sign-in service, which they're pushing aggressively onto apps on their iOS platforms. It's seamlessly integrated. The privacy-focused search engine DuckDuckGo is now using their duck.com address for a [burner email service](https://spreadprivacy.com/introducing-email-protection-beta/). Last year, Mozilla launched [Firefox Relay](https://relay.firefox.com/) as a free tool for doing burner emails as well. And just today, the popular independent email service [Fastmail](https://ref.fm/u25459520) (it's like Gmail, but you pay a little for it instead of having ads) announced that they were teaming up with the popular password management app 1Password in order to offer a similar burner email service.

Each of these services has a slightly different user experience and feature set, but the overall result is that *millions* of people have suddenly disappeared from the email-based surveillance tracking systems of the internet. Their addresses each seem unique and unfamiliar to those looking to creep on their data. The organized, hyper-connected data streams are now polluted with what look to be millions of new addresses that have no recognizable history. To be sure, the connection between a particular identified user and their new, burner email could still be reverse-engineered by the big ad networks, but it's a lot more costly and complex to do so. And while they work on that problem, the burner email services will work on making their offerings even more ubiquitous and easy to use. It's the first time in decades that privacy advocates have a meaningful technical advantage over the trillion-dollar ad platforms.

## Avoiding The Paparazzi

In this week's New Yorker, Chris Hayes makes a strong argument about the ubiquitous surveillance culture of today's social media world, but it's grounded more in the psychological impact of our words and actions always being on display. In his formulation, [we're always famous](https://www.newyorker.com/news/essay/on-the-internet-were-always-famous). I liked this perspective on its own merits, as it's an important point for everyone to understand on its face, but I also think it's strongly paralleled in the impacts that surveillance-based tracking systems have on our lives. In addition to hyper-vigilance about our words being taken out of context, or resurfaced after our views have evolved or norms have changed, we also have a subconscious (fully justified!) paranoia about the way our actions are being tracked by monetization platforms.

In both cases, we know there are harms associated with digital hyper-visibility. 

<blockquote class="twitter-tweet" data-dnt="true" data-theme="dark"><p lang="und" dir="ltr">wowwww</p>&mdash; Chris Hayes (@chrislhayes) <a href="https://twitter.com/chrislhayes/status/1442326721278054401?ref_src=twsrc%5Etfw">September 27, 2021</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

The answer lies in a drum that I, and many others, have been banging on for decades now: [privacy through identity control](/2002/12/17/privacy_through/). Though some parts of that piece from 2002 haven't aged well (here's me wincing at the passing mention of fascist ghoul Rudy Giuliani), there are some core points that I think are more pertinent than ever:

> ****We’re all celebrities now****, in a sense. Everything that we say or do is on the record. ... Do we have to permanently filter our thoughts and expressions, lest they be thrown back at us at some inopportune moment in the future? What do we do until people are used to seeking out context, until meta is intrinsic? Well, you have to own your name. I own my name. I am the first, and definitive, source of information on me.

> One of the biggest benefits of that reality is that I now have control. The information I choose to reveal on my site sets the biggest boundaries for my privacy on the web. Granted, I’ll never have total control. But look at most people, especially novice Internet users, who are concerned with privacy. They’re fighting a losing battle, trying to prevent their personal information from being available on the web at all. If you recognize that it’s **going** to happen, your best bet is to choose how, when, and where it shows up.

This is a refrain I've kept coming back to in my work, both personal and professional, all these years. There's something meaningful, profound and empowering about having ownership and control over one's self and what happens with one's words and actions. It's the only form of personal protection that scales, and it's the bedrock of agency and empowerment against institutions that would seek to exploit.

We don't yet have an easy, automated way to defend ourselves against all the potential harms of the digital world. We'll never have one that's 100% effective. But today, for the first time in a long time, we have a chance to take the first few of those thousand little cuts that might help us take back a little bit of what should have been ours all along.
