---
title: A middle layer of web apps
slug: a_middle_layer
date_published: 2004-08-19T15:53:35.000Z
date_updated: 2004-08-19T15:53:35.000Z
---

Olivier has offered a challenging analysis whose name explains his thesis: "[Organizr is Nice, But Not a Web App](http://www.oliviertravers.com/archives/2004/08/18/organizr-is-nice-but-not-a-web-app/)". The fundamental debate is whether an in-browser Flash app that calls a RESTian web service is a "real" web app in the same sense that an HTML app is.

My initial thinking on this is:

# A management application running in Flash is actually in a slightly different class, a middleweight interface halfway between a thin-client HTML page and a rich executable client.

# Who cares?

Stewart makes a fairly compelling argument that the real-world web consists of anything that sits on top of it. I’ve [talked about creating web apps that are valid XHTML](http://www.alistapart.com/articles/typepad/), and interestingly the reaction from people commenting was to focus on whether an application’s *output* was valid, with the markup of the application’s actual user interface seeming almost unimportant. That’s completely understandable, but it underscores the "Who cares?" point by refocusing on what comes out of the application, instead of the technical specifications of the application itself. Even if Olivier’s right, it doesn’t change anything.

The more interesting part to me is the layering over web services that we’re seeing. [DropCash](http://www.dropcash.com/) is the definitive example right now, [reusing existing APIs](http://www.sixapart.com/log/2004/08/dropcash_launch.shtml) like [TypeKey](http://www.movabletype.org/docs/tk-apps.html) and PayPal to provide a useful and unique service. But the potential for building even more on top of these second-level platforms is the reason that I’m excited about DropCash.

I want enough APIs built on top of DropCash that I can build (or rather, one of the PBs can build) a wishlist gifting tool. Give the service a person’s name, and it goes to their site and finds their Amazon wishlist link, maybe from their FOAF file. Using the Amazon API, you grab the person’s wishlist, enumerate the items, and sort them by price, lowest to highest. Create a DropCash campaign that ends on a certain date (the giftee’s birthday?) rather than at a certain dollar amount. Retrieve the images of each item on the wishlist and line them up next to the bar chart showing the campaign’s progress.

Then it’s all about notification. All of you who thought "DropCash needs an XML feed!" rest assured: [Andre](http://notes.torrez.org)‘s thought of that, I’m sure. But this campaign could update donors either via subscription or email and say "We’ve raised enough money to buy a CD!" or "…to buy a TV!" or "…to buy a PC!". *That’s* a useful layering of web services. Wishlist gifting app on top of Amazon on top of DropCash on top of TypeKey on top of PayPal. Nothin’ but net.

Should you do it in a Rich Internet App or a thin client or a dedicated desktop app? I don’t much care. If you do it right, it’s easy enough to plug any of those into the service you’ve created. Do one reference implementation, and let the Lazyweb build the rest of the versions and improve upon what you’ve done. Let a thousand clients bloom. [Web as OS](http://www.kottke.org/04/08/web-platform) or whatever.

Naturally, I love [Organizr](http://www.flickr.com/tools/organizr.gne) because it’s a cool app. But I don’t just want it to talk to the [Flickr API](http://www.flickr.com/services/api/). I want to layer it on top of the Atom API and see my posts in the same view that I see my images. Timeline slider that scales and shows posts within a certain range.

Then, stack Organizr on top of the Wishlist app. I want to see pictures of each of the gifts that’s been given away on campaigns that were created in the last month. And then…?
