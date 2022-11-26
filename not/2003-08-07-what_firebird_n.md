---
title: What Firebird Needs
slug: what_firebird_n
date_published: 2003-08-07T13:51:14.000Z
date_updated: 2019-11-10T08:19:38.000Z
tags: tech
---

My recent [ranting about fonts](http://www.dashes.com/anil/index.php?archives/006837.php) notwithstanding, I’m usually seen by the web development community as a Microsoft apologist. I use (and *like* using) Windows and my main browser is Internet Explorer 6.0.

That statement usually inspires all kinds of brilliance in correspondents, ranging from "M$ blowz!" to "bet u get hacked lol". But I keep up with security patches, have a firewall, and the Google Toolbar blocks popups sufficiently for my tastes.

Despite this confession, I will enthusiastically concede that [Firebird](http://www.mozilla.org/products/firebird/why/) is a fantastic browser. After some initial rough spots, Ben Goodger created a terrific advocacy page explaining the browser’s benefits. And it warms my heart to see people like Asa working on [integrating Movable Type into web panels](http://weblogs.mozillazine.org/asa/archives/003810.html). That’s exactly the kind of innovation that gets people hooked on a tool. I spent a while trying to hack my Movable Type boomarklet to load into Internet Explorer’s search pane, and while I was successful, it was nowhere near as pleasant an experience as a well-designed XUL form would be.

But all that praise aside, IE’s still been my default browser thus far. So starting today, I’ve set Firebird as my default so that I can focus on the shortcomings that explain why I haven’t yet switched. Now that the [Google toolbar](http://googlebar.mozdev.org/) on Mozilla and Firebird has reached parity with the official toolbar for IE, my major obstacle is overcome. The extensions support in Firebird is fantastic and gives me hope that most of the new features I need will be added quickly, along with the fact that there are [dozens of others available](http://texturizer.net/firebird/extensions.html) which I hadn’t even known I wanted.

What don’t I have? I think the primary missing pieces are context menu additions that could probably be created for Mozilla, but that I don’t have the time and inclination to learn how to create, especially when they’re easily added to Internet Explorer. The first gee-whiz feature (people are always amazed when they see this and don’t know it exists) that I use constantly in IE is the ability to highlight a selection on a web page and right-click to view source for just that part of the HTML for the page. It’s just one of several great features in [Microsoft’s Web Developer Accessories](http://www.microsoft.com/windows/ie/previous/webaccess/webdevaccess.asp) that are free to download.

Also critical are a few features afforded by the [IE Web Accessories](http://www.microsoft.com/windows/ie/previous/webaccess/ie5wa.asp), such as right-click highlighting of text on a page and the ability to zoom in and out on an image (which just involves resizing the image by 50% or 200%) by right-clicking on it.

A few years ago, I talked to [Dan Sanderson](http://www.dansanderson.com/blog/) about his [BlogTracker](http://www.dansanderson.com/blogtracker/) tool, then known as Subhonker Filter, and he created the ability to view update lists in the IE sidebar, which simply involves setting the TARGET attribute of a link to "_search".

Since then, I’ve created a bunch of tools for my personal use which load into the sidebar in the same way, which works great on my widescreen laptop, since it still allows me to see a full web page while the sidebar’s open.

So a common theme seems to emerge. I use right-click extensions and I use a lot of tools which load into the Search Pane in the browser. It seems like the latter need could be met by having Firebird web panels support the target=”_search” syntax, even though it’s not a standard, so that those links would work without changing the syntax from IE. The right-click extensions are certainly possible in Mozilla-based browsers, but they’re completely incompatible with the way that IE implements them. So there’s probably some demand for recreating a handful of context menu features.

I’ll keep posting as I find other elements of my surfing habit that Firebird doesn’t support yet (bookmark handling is still weaker in Firebird, too) but feel free to add your own list of requisites here if you’re still using IE as your primary browser.
