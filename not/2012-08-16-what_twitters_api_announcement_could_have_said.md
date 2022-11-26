---
title: What Twitter's API Announcement Could Have Said
slug: what_twitters_api_announcement_could_have_said
date_published: 2012-08-17T02:48:24.000Z
date_updated: 2012-08-17T02:48:24.000Z
tags: tech
---

A few years ago, I wrote about the [Law of Fail](http://dashes.com/anil/2009/06/the-end-of-fail.html): Once a web community has decided to dislike a person, topic, or idea, the conversation will shift from criticizing the idea to become a competition about who can be most scathing in their condemnation.

This is relevant today because Twitter announced some [upcoming API changes](https://dev.twitter.com/blog/changes-coming-to-twitter-api). From my standpoint, these are mostly pretty reasonable, and in fact should have almost no impact on any normal Twitter user. Naturally, super-geeky developers are incensed. And of course, the people who most eagerly participate in the pile-on usually have the least skin in the game — they just want to complain.

But to be fair, a valid annoyance for developers is that the communication from Twitter about these kinds of changes has been vague enough to leave them uneasy. Combine the tech blogosphere’s Law of Fail behavior with the tendency that crowds have toward assuming the worst rumors in any given situation must be the truth, and you have a recipe for panic.

So, as an exercise in radical institutional empathy and the real-time exploration of alternate histories of the tech industry, I wrote *my own* version of the Twitter API 1.1 announcement.

My goal is to communicate the exact same points, but with the clarity that would inspire the least amount of [user-generated discontent](http://dashes.com/anil/2007/08/inspirational.html) possible. It’s also shorter by about 500 words and omits the 2×2 grid of API clients. Edits, corrections or criticisms are welcome!

---

### Our biggest Twitter API upgrade ever

We have awesome news for Twitter developers: Today we’re announcing the upcoming release of the biggest new set of features and changes to the Twitter API ever, which we’re calling Twitter API version 1.1. We know change is scary, so we’ll talk about what’s new, why we’re making these changes, and when you can expect to see them. Don’t worry — it’ll be worth it!

The TL;DR version of what’s new:

- More API calls for almost every kind of app, with per-endpoint rate limits
- Better security by extending OAuth to all APIs
- A clear roadmap for Twitter app developers to know what’s encouraged, including detailed instructions on how to show tweets and timelines
- A few new restrictions for people making traditional Twitter clients
- When version 1.1 is officially released, you’ll have six months to migrate from API version 1.0

### Huge increases in API call limits:

In today’s API 1.0, we limit authenticated API requests to 350 per hour. Good news: We’re going to blow that limit away for your apps providing 60 calls per hour per endpoint – so you can literally hit every different endpoint every minute and not go over the rate limits. Endpoints that are *really* in demand, like Tweet display, profile display, user lookup and user search go all the way up to 720 calls per hour.

This is a big increase for almost every kind of app, and we’ll give you the full details of the new extra-legroom limits when API 1.1 is released.

### All Auth Everything

The big new API call limits come with only a minor change in what’s required from you: You’ll have to use OAuth for *all* of your API requests. This shouldn’t be a big deal because it works the same way as the OAuth requests you’re already making. (If you are not yet using OAuth, OMG shame on you, you’ve got until March 2013 to get with the program.)

An awesome side bonus of this new auth regime is that people who are abusing the Twitter ecosystem we all share by scraping or writing spammy bots or other annoying behaviors will be able to be reined in using their auth tokens, instead of the brute-force block-by-IP method we’re stuck with now. Here’s crossing our fingers for less spam!

### We Love Your App!

Sure, there’s been some hand-wringing about what direction we’re headed with our API, and whether third party developers are “safe” working on Twitter. Good news: Your app is welcome here, and we appreciate you developing on Twitter.

In order to make sure we don’t ever get the community worried again (and to hopefully stamp out some of the scarier rumors that pop up in the ever-reliable tech press), we want to give some detailed outlines of how to make sure you’re in the clear while working on the Twitter API.

Obviously, our greatest wish is that your app is hugely successful on Twitter, and we of course need to make sure to support our business model, including promoted tweets and sponsored tweets and whatever else we come up with.

So, the first thing we’re doing is offering up detailed documentation of how tweets and timelines have to be displayed when using the new 1.1 API. This is mostly to ensure a consistent, simple interface for users who are hopefully switching between lots of cool Twitter-powered apps, including yours. But this also cuts down on apps that introduce confusing buttons or UI to try to pull people out of their Twitter experience, and makes sure the advertisers who actually pay for this whole thing to run get what they’re expecting, too.

You can read [the guidelines](https://dev.twitter.com/terms/display-guidelines) on your own, but the bottom line is that Tweets will start to look really consistent everywhere. That also means that apps which deliberately try to change the way Tweets or the Twitter UI looks can be shut down, so don’t do that.

Oh, and if you need a *lot* of user tokens (like, more than 100,000), get in touch with us and we’ll take care of you personally. If you try to make that volume of calls without a special request, you might get shut off.

### A Note On Traditional Twitter Clients

The only kind of Twitter app which has real constraints under API 1.1 is traditional Twitter posting clients — ones that offer the basic reading and writing experience and little else. While we appreciate these apps (our own official Twitter clients started out as one of these!), the reality is it’s going to take more effort for third parties to maintain these apps than it has in the past, because we’re going to be very strict about requiring updates to make sure your clients are in compliance with the user experience standards we set in our own first-party apps.

Put simply: If you have made a traditional Twitter client, you’re going to be expected to hew very closely to our new display guidelines and will regularly be asked to make updates about the way you display content, sometimes with short notice. We recognize that might cause additional costs or stresses that make it less rewarding or more frustrating for this small but important community of developers, but this is essential for building a robust, successful Twitter business to support us all, and for us to shut down the small but persistent number of developers who use this kind of access to make spammy apps that degrade the Twitter experience for everybody. Client apps that don’t keep up with these standards or that fail to immediately reflect changes that are required will have API access cut off.

That being said, many third-party Twitter clients have dedicated user communities and passionate developers, and with focus on keeping in step with our evolution, they should continue to thrive with their audiences.

People making stats apps and analytics tools and social media marketing platforms all have absolutely nothing to worry about — the vast majority of Twitter client apps will move to the new 1.1 API with no changes expect better auth and higher API limits.

### More To Come!

We’re excited about the apps you’re going to build on the new APIs, and we’ll be unveiling even more powerful features for you to incorporate features like Twitter Cards which will make your apps and sites even more engaging. In the meantime, if anything in this announcement is unclear, let us know in the forums or by @replying to us on Twitter, and we’ll answer any questions you have.
