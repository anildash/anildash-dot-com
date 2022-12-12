---
title: Apple's Twitter
slug: apples_twitter
date_published: 2011-06-01T03:58:30.000Z
date_updated: 2011-06-01T03:58:30.000Z
heroimage: https://cdn.glitch.global/c4e475b2-a54e-47e0-973c-ed0bd1b46262/apple-twitter.png?v=1670802785093
tags: [tech, apple, twitter]
---

I’ve been waiting a year for someone to write about this, but my laziness has not yet paid off, so here are a few things that we all know about everybody’s favorite Cupertino fruit company:

- Apple has client app software on hundreds of millions of devices in the form of iTunes on PCs and Macs and, well, all of the bundled software on iOS devices.
- Apple has an extremely large-scale realtime messaging service, in the form of [Apple Push Notifications](http://en.wikipedia.org/wiki/Apple_Push_Notification_Service), which has scaled with high reliability to what must be an extremely large number of messages, certainly on the order of hundreds of millions a day.
- Apple has account info for every person receiving those notifications, usually including credit card information.
- Apple has lots of experience making client applications for short-length interpersonal messaging.
- Apple has a proven ability to get the attention and interest of artists and tastemakers who influence culture and inspire a following.

And here are a few things which Apple doesn’t have:
- Any success or demonstrated ability in making compelling clients for social networking, whether in the form of Game Center or Ping.
- A usable API for developers to build on this realtime networking infrastructure in a lightweight way in web apps, or in languages other than Objective C.

To some degree, third parties like [Boxcar](http://boxcar.io/) address some of the need for a generic push notifications client; Services like [Urban Airship](http://urbanairship.com/products/push-notifications/) solve a good bit of the API problem as well.

But in short, the hardest, most expensive technical part of building a web-scale Twitter competitor already exists in Apple’s infrastructure. What’s missing, in an odd reversal of Apple’s usual pattern, is a well-designed, simple user experience that makes people want to participate.

Could a small team of developers and designers within Apple make a credible realtime messaging service with first-rate native clients on every important platform? Could they graft on a simple, REST-based web-style APIs to the complicated, old-fashioned API that enables push notifications right now? It’d be a lot like building a usable, delightful user interface on top of well-established, but complicated, technological underpinnings, wouldn’t it? I wonder if Apple has those skills.

Related:
- [Delivery as a Service](/2010/12/delivery_as_a_service)
- [The Pushbutton Web](/2009/07/the_pushbutton_web_realtime_becomes-real)
