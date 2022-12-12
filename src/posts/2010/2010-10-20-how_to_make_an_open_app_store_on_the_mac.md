---
title: How to Make an Open App Store on the Mac
slug: how_to_make_an_open_app_store_on_the_mac
date_published: 2010-10-20T18:40:39.000Z
date_updated: 2010-10-20T18:40:39.000Z
tags: [tech, apple]
---

Apple took the not-very-surprising step of announcing an App Store for Mac OS X, an idea I was [ruminating about](/2010/10/20/all_the_app_stores) earlier today in looking at all the app stores available today. So, now that we know that it exists, how do people who are concerned about the openness of the Mac OS X ecosystem for third-party developers make sure that Apple doesn’t get a total stranglehold on app distribution on the desktop?

It’s actually quite doable, if two unheralded but influential independent projects coordinate their efforts, or even merge. Their quiet ubiquity among third-party applications could create an emergent app store, turning a broad base of already-distributed and successful independent apps into a force with a lot more marketing and bargaining power in their discussions with Apple. So, who has the ability to change the balance of power here?

- [Sparkle](http://sparkle.andymatuschak.org/): Andy Matuschak has made a library called Sparkle, which allows any independent app to automatically announce and install app updates. If you’re a serious Mac user, it’s already on your system — from Transmission to Stuffit to Adium to TextMate to NetNewsWire to Evernote and on and on, many of the most popular apps on the Mac desktop all use the same tech for the critical app store functions of updating and alerting users to new versions.
- [Growl](http://growl.info/): Growl is a ubiquitous and enormously popular open source library for announcing system events on Mac desktops. You can [browse the list of apps](http://growl.info/applications.php) that use Growl for yourself, but again, you’ve probably already got it on your system. It does a much broader range of notifications than the simple app updates notices of Sparkle, but it also has an even larger installed base. It’s not strictly tied to app store functions, but it has the distribution that could be leveraged to give independent developers an extremely broad base of market penetration among Mac OS X users.

### The Strategy

So, given these bits of software are useful, have key app store functions built in, and are on an enormous number of Mac users’ systems already, what would it take to create an app store to compete on a nearly-level playing ground with Apple, while ensuring that independent developers retain ultimate control of their works and distribution?

Here’s a rough outline of the steps that would need to happen:

- **Move quickly**. A number of prominent app developers would have to commit to supporting an open mac app store, by making their apps available on that store. These announcements would pretty much have to happen this week in order to have enough impact to sway the course of discussion. There’s no reason these would have to be exclusive, or say anything negative about Apple’s app store, but could just be expressions of these developers pursuing every distribution option available.
- **Don’t waste time in committee**. Being Mac developers, their overwhelming impulse will be to waste time making pretty icons, endlessly debating the name of this new app store, and losing time to all manner of distractions which aren’t actually that strategically important. This opportunity will only succeed if devs stay focused, don’t waste time Dribbbling on themselves, and aren’t trying to write a new galactic constitution. Make a simple wiki page or something, and list your names and apps.
- **Make payment infrastructure part of Version 2.0**. These developers have succeeded in the market without creating one Grand Unified Shopping cart, and they’ll be able to continue to do so if they don’t try to solve the payment problem right away. Let that be a great, innovative part of Apple’s store for now, so that you can get this thing to market.
- **Have the “app store” experience live within each of the apps themselves**. To maximize the distribution benefit that each developer provides to the others, don’t try to turn Sparkle or Growl into an app store with a dock icon of its own. Instead, make an embeddable store experience that could live within a menu option in the apps themselves, perhaps providing contextual suggestions of “other users who use this app also liked these other apps”.
- **Don’t make it about Apple**. One of the biggest temptations will be getting drawn into long, pointless conversations about “the meaning of open” and “the benefits of integration” and other highfalutin’ horseshit, or to be stuck attacking or defending Apple. That’s great Gruber fodder, but it won’t help you in making an app store that actually gives you some leverage with Apple. Don’t write long blog posts about The Meaning Of The Lion App Store if you could be just working on something to help you and your fellow developers.
- **Ship before Lion does**. If you can’t do that, shame on you.

So, independent Mac developers: I’m an eager customer of your products. I want to give you my money. I also want you to stay empowered and able to make your own decisions about how your products are distributed. Give these suggestions some thought, point out any omissions or errors I’ve made, and start announcing your plans to defend your independence. Good luck.
