---
title: Clouds for People, or the Consumerization of the Cloud
slug: clouds_for_people_or_the_consumerization_of_the_cloud
date_published: 2012-06-28T17:52:22.000Z
date_updated: 2012-06-28T17:52:22.000Z
heroimage: https://cdn.glitch.global/c4e475b2-a54e-47e0-973c-ed0bd1b46262/google-cloud-engine.png?v=1670724296899
tags: [tech, web]
---

Right now, there’s no App Store for Amazon EC2. Today’s just-announced “[Google Compute Engine](http://cloud.google.com/)” isn’t plugged in to Google Play, the Android Music and app store. Microsoft seems to be moving toward unifying the various Windows and Zune and XBox stores into one great super-store of content, but stuff that lives on the Azure cloud is a world apart.

I don’t think that’s going to last.

The simple consumer model of one-click buying of app experiences at low prices is, happily, here to stay. But currently, those apps can only be bought for mobile devices (phones and tablets have very mature app stores) and are just starting to become available on desktops through the Mac app store (I [had some feelings](/2010/10/how-to-make-an-open-app-store-on-the-mac) when that was announced two years ago) and the upcoming Windows 8 store. The television/gaming consoles like XBox, AppleTV, GoogleTV and the rest have pretty robust app stores, too, of course.

There’s an entire class of innovation that’s being ignored by focusing on just these consumer devices, though. Cloud computing is getting increasingly powerful and rapidly decreasing in price, but right now the only beneficiaries are a narrow class of enterprise and developer technologists. Apps that have the always-connected, high-bandwidth, compute-intensive, storage-hungry traits that make them a perfect fit for today’s cloud consumers might make a *great* experience for a lot of regular individual users. We see that today with the awesome potential of platforms like [OnLive](http://onlive.com/), which uses the cloud to bring those expensive elements of computing to much cheaper devices.

So we need a consumer cloud offering. An app store for EC2 or a marketplace for Rackspace. The same one-click stores that offer us easy apps on our own local devices should let us purchase consumer-friendly apps that run on our own individual cloud servers.

## EC2 For Poets, And For Other People

Sure, regular folks having their own cloud computing accounts might seem more complicated or esoteric. If you wanted a service that runs on other people’s computers, wouldn’t you just sign up for a centralized site like Facebook or Gmail or something? Maybe not.

First of all, I’m not suggesting that regular consumers (or even power web users) should be exposed to the super-technical management interfaces that current developers and administrators face when working with cloud infrastructure, whether it’s platform-as-a-service or infrastructure-as-a-service.

Instead, newer cloud providers like [Digital Ocean](https://www.digitalocean.com/) or [AppFog](http://appfog.com) (or even friendlier versions of offerings from existing providers like Heroku and Rackspace) point the way towards experiences that regular people might actually want to use. In a way, these platforms would be the successors to the mom-and-pop web hosts that used to be used to run all kinds of one-off apps a decade ago before the web hosting market consolidated.

For years, [Dave Winer](http://scripting.com/)‘s been talking about “EC2 for Poets”, the idea of getting Amazon’s web services platform running for regular liberal-arts-leaning folks. I agree with his fundamental premise that only arrogant techies think their platforms are beyond the grasp of normal users.

But I *do* think many people who would benefit from these kinds of platforms just don’t want to invest that kind of time in learning. More importantly, **incredible innovations in features and user experience emerge when you moving computing power to the edges of the network**.

Through this lens, a huge part of the entire mobile app phenomenon that iPhone really catalyzed is merely an impact of moving so much computing power to the edge of the mobile phone network, instead of trying to provide so many services through archaic centralized infrastructure. Put simply: Move the brains to the edge of the network, and you get great new kinds of apps. We don’t know what the Angry Birds or Draw Something of the server-side web app world looks like right now, because right now there’s no way for consumers to buy it.

## Regular People Having Web Servers?

Now the skeptics reading this will say, “Who in the hell is gonna want their own cloud server to run an app when they could just sign up for a simple centralized service?” First, I am supposing that the sign-up and account creation experience for these services could be made as simple as signing up for Facebook or iTunes or other payment services.

But second, I *know* there’s an entire class of applications that centralized services don’t create. Every day, a dozen different people at Google or at Facebook or at Twitter say to each other in a meeting, “Well, that’s a great feature, but only one percent of our users would want it, and it’s super compute-intensive, so let’s just table that for later.”

Unless some enterprising and generous engineer devotes their slack time to creating the feature out of sheer enthusiasm, those ideas die. Not because of merit, but because we have no option in between intermittently-connected, low-bandwidth personal devices and centralized megaservices with unified, homogenous feature sets.

No two people’s smartphones have the same functions, thanks to app stores. Everyone’s web sites have the same features, even *despite* platforms like Facebook’s apps, because those apps have to live within the constraints of what Facebook permits and can support.

So there’s a third way. Hopefully a robust and enthusiastic multi-front war between the giant cloud players like Amazon, Google, Microsoft, Rackspace, platform efforts like Cloud Foundry and OpenNebula, and enablers like Jumpbox and Bitnami and [Cloudstore](https://cldstr.com/) will yield benefits not just for big companies, but for regular users, too.

There’s no reason the experience can’t be as seamless and easy to buy an EC2-hosted web app on a Kindle Fire as it is to buy Words with Friends or the Foursquare app. Of course, we’re starting to experiment with the first steps towards this ourselves on ThinkUp. We’ve been trying out a [simple cloud setup](https://phpfog.com/thinkup?a_aid=24990363) for ThinkUp that gets people up and running with the app on PHPFog’s infrastructure in a few minutes. We make a couple bucks, they provide a great infrastructure, and semi-technical users get an experience that, while not quite as easy as point-and-click in iTunes, starts to hint at how a whole new app ecosystem could work.

## Related

Showing some of this evolution, from two years ago, a list of [all the app stores](/2010/10/all-the-app-stores). It’s a very different perspective on the then-current application platforms, before we’d realized that some of them were app stores in disguise. Of course, some of those platforms still don’t know that they’re app stores.
