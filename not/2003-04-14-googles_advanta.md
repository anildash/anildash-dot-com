---
title: Google's advantage is RAM
slug: googles_advanta
date_published: 2003-04-14T21:48:14.000Z
date_updated: 2003-04-14T21:48:14.000Z
tags: tech
---

**Update:** Read the comments. Dan and Joshua, who know way more about this stuff than I do, explain why I’m wrong and help me clarify what I’m really asking for. Smart guys, and great ideas.

One of the recurrent complaints about desktop search as compared to the standard set by Google is that finding one’s own files is so much slower. If Google can index a couple billion pages and return the results in .03 seconds, why does a search of my hard drive take 30 seconds? We know that we’ll put up with the search being 3 orders of magnitude slower because our own information is 3 orders of magnitude more important than the random fluff on the web, but how can we make it work *better*?

Well, Google’s secret is no secret at all: It’s RAM. Random Access Memory. Just like you’ve got in the machine you’re using right now. Keep in mind, all the thousands of boxes in Google’s racks do all their querying in RAM. Even with network latency and the time it takes to send a request to their data center and with the index encompassing terabytes of data, RAM is just that much faster. The downside, of course, is that keeping data in RAM requires redundancy, since it loses its contents as soon as the power is cut. Indeed, Google’s people have said that one of their primary logistical concerns is the massive amounts of power needed for supporting and cooling all those RAM-hungry boxes. But if the couple hundred megabytes of information that you value were all available in RAM, your search times would be even faster than Google’s.

So, how can this be done? Well, it’s not hard. PCs have had a driver for RAM drives available since the days of DOS 3.0. But improvements in Windows’ memory paging system made RAM drives obsolete. Still, Microsoft offers a [sample RAM disk driver](http://support.microsoft.com/default.aspx?scid=http://support.microsoft.com:80/support/kb/articles/Q257/4/05.ASP&amp;NoWebContent=1) for Windows 2000, and even includes a version of the driver in XP, though you have to manually install it to activate it. Or you can download a [free third-party version](http://www.arsoft-online.de/products/product.php?id=1) of the same driver, complete with installer.

(Side note to XP users, if you try to activate the driver: If you don’t have any disks with the FAT file system, the driver won’t work, as it uses FAT for the newly-created drive. You’ll need to [enable the fastfat driver](http://pub29.ezboard.com/fcyberwizardfrm20.showMessage?topicID=16.topic) to make use of it.)

I tried a few experiments, moving my browser cache to the RAM drive, or moving my temporary files there, or even moving my entire email archive to RAM, and it turns out to make a massive difference in performance. Nearly everything is instant. Running a copy of Photoshop installed to the virtual drive is astonishing the first few times you start the app. But it’s not a solution that really works for any length of time, as various parts of Windows balk at being run from a drive that’s not "real". And you don’t want to have to reinstall your apps every time you reboot, even if XP only rarely needs to be rebooted.

So what good does this insight into Google and RAM drives do us? Well, it seems like there’s an opportunity. Someone with just a little bit of time and ingenuity, who’s interested in making tiny apps like [Andre](http://www.torrez.org) does with [torrez.net](http://www.torrez.net) could easily make an installer for a RAM drive that caches important, frequently-accessed data in RAM in a way that preserves its state by writing it to disk upon shutdown. Perhaps with a backup system that mirrors the RAM disk to the hard drive when the system is idle. The fact that RAM is so volatile could probably be compensated for, or even sold as a benefit. ("Your browser history is *permanently erased* every time your computer shuts down, for the ultimate in security!") And a My Documents folder mirrored to this storage area would be searchable with Googlesque speed.

I’d be willing to beta test it. I work on a laptop, so even if the power cuts out, my battery acts like an uninterruptible power supply, preserving my system’s power source. And I’d pay, I dunno, $30 or something for the simple software, along with another couple hundred bucks for enough RAM to copy everything useful to memory. I bet there’s a market.
