---
title: Delivery As A Service
slug: delivery_as_a_service
date_published: 2010-12-20T19:30:32.000Z
date_updated: 2019-09-25T05:46:13.000Z
tags: tech
---

Since a few people told me they found my notes on [cloudtop applications](http://dashes.com/anil/2010/09/cloudtop-applications.html) useful when I posted them a few months ago, I thought I’d share some more notes in the same spirit. Part of my immediate motivation was when my friend Andre wrote up some [notes on building a web-scale app in a weekend](http://notes.torrez.org/2010/12/learn-to-program-in-24-hours.html), Jason Kottke made a [smart mention](http://kottke.org/10/12/on-weekend-web-apps) of the difficulty of delivering messages, as evidenced by [Jeff Atwood’s post](http://www.codinghorror.com/blog/2010/04/so-youd-like-to-send-some-email-through-code.html) earlier this year. If these smart folks are struggling so much, surely there must be another option?

Well, I’ve noticed a pattern that suggests there is a better way. This time it’s not a pattern in end-user applications, but rather in infrastructure services, which I’d call “Delivery as a Service”. In this model, new offerings provide a set of message delivery services for developers that share a few common traits:

- Digital services that pre-date the web, or were designed without the web in mind, can now be exposed as simple web services
- Legacy platforms that require extremely expensive startup costs convert into a cost-per-message (or cost per thousand messages) model
- Message systems with effective anti-spam components usually exert a high cost on spammers that can also be a prohibitively high bar for small developers unless they’re able to pool their efforts
- Service providers can aggregate requests from many small, separate applications to make costly services approachable for independent developers
- You can figure out what the hell these service providers *do*, unlike many generic web service providers

With those traits in mind, who’s providing Delivery as a Service systems now? I’m sure this is a far-from-comprehensive list (suggestions very welcome!) but these are the few that got my gears turning:

- [Urban Airship](http://urbanairship.com/): Love these guys. Primarily focused on doing push notifications to iOS-powered Apple devices, they’re rapidly expanding into related in-app sales, rich-notifications, and other areas. While Apple does offer an API for its notifications, it’s not as easy to use and web-friendly as UA’s offerings, and they handle much of the other infrastructure requirements that would otherwise be onerous.
- [Postmark](http://postmarkapp.com/): Good old-fashioned email! It turns out that, these days, delivering email that doesn’t get marked as spam is actually kind of a pain if you’re not a huge provider. And much of the commercial email market it optimized for direct marketers. But Postmark has an interesting niche in providing the valuable email capability for developers that don’t want to spend precious development cycles on boring-ass email.
- [Twilio](http://www.twilio.com/): Perhaps the most impressive of the bunch. Twilio handles voice, IVR and SMS functionality for many apps, with a really simple API that any developer can work with.

Now, individually, none of these capabilities are particularly new. (Though of course, iOS push notifications have only been around a relatively short period of time.) But making them broadly available, accessible through simple APIs with code libraries available in common programming licenses, and having initial access be available for pennies or even for free? *That* represents a big change.

### Tomorrow’s Implementation of Yesterday’s Technology, Today.

With the proliferation of these services, features that would be “someday” or “after we get funded” features can be pushed up much earlier in a product’s lifecycle. And markets that would otherwise be underserved are now approachable; Every company that’s putting money into developing an iOS app around their services could use Twilio to provide a robust SMS-based interface at the same magnitude of cost. The early signs of success for each of these little companies is promising too; It might inspire bigger infrastructure providers like UPS (which has its own [API for shipping services](https://www.ups.com/upsdeveloperkit)) to market their services more like these startups as well.

I find delivery services most compelling in the context of how they serve the “[cloudtop](http://dashes.com/anil/2010/09/cloudtop-applications.html)” apps I described a few months ago, but I can see these being equally important for enterprises or other environments as well. We need more simple services to connect to the real world, to “old-fashioned” technology that isn’t web-centric, but that could still be enhanced by being connected to the web. Making a RESTful API for faxing might not be sexy, but it could enable some businesses to reach new audiences or do something creative with all of those underutilized rolls of thermal paper. If you can think of services like this that should exist, or if you’ve built one, let me know in the comments.
