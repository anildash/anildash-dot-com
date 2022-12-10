---
title: Tidy for ActiveX
slug: tidy_for_active
date_published: 2003-10-08T17:15:39.000Z
date_updated: 2003-10-08T17:15:39.000Z
tags: tech
---

Given the fact that [Macromedia](http://www.macromedia.com/devnet/activecontent/articles/devletter.html) and [Microsoft](http://msdn.microsoft.com/ieupdate/) have both listed the changes coming up for working around the Eolas-mandated modifications to Internet Explorer, we’re going to be seeing millions of web pages changing in the next few months.

I’d guess most companies will start seeing a rash of error reports ("Why do I get a popup on your site?") around January, and then they’ll want to start moving all their OBJECT tags to javascript document.writes. Macromedia’s announced that they’ll be creating a tool to automate this, I assume Microsoft will as well, and it would seem likely for Real and Apple’s QuickTime group to follow suit.

So there’s an opportunity here, if you’re committed to [web standards](http://www.webstandards.org) and want to make a real impact. Start working with [HTML Tidy](http://tidy.sourceforge.net/) and make a version with a simplified UI, which creates valid markup and fixes OBJECT tags in one fell swoop.

There’s a real potential for this tool, if done right. A free, vendor-neutral application which fixes pages simply and easily for inexperienced users and small businesses (it should be able to remote FTP into a site and fix all the pages from the desktop) has the potential to make millions of web pages forward compliant. And given the fact that it will be web developers performing this task, we have enough influence that ActiveTidy could rapidly become the de facto standard for this kind of repair work.

There is also an opportunity for a web service which would allow you to provide your server login information so the service could remotely update your site, but that’s an arrangement that only the least technicallly savvy would be comfortable with.

So, for you great developers out there, go see if you can take Eolas’ breakage of the web and help turn it into an opportunity to fix millions of HTML documents.
