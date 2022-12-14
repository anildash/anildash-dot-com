---
title: fixing web pages on the fly
slug: fixing_web_page
date_published: 2003-01-14T21:00:55.000Z
date_updated: 2003-01-14T21:00:55.000Z
tags: random ha-ha
---

I was thinking about the fact that [browsers have to fix up a page](http://ln.hixie.ch/?start=1037910467&amp;count=1) internally in order to render it correctly if elements are incorrectly nested or are left unclosed. Since we know that Mozilla does a pretty good job of this, and its fix-up engine is open source, shouldn’t it be possible to make a web proxy that feeds a tag soup source HTML document through the fixer-upper and outputs a valid XHTML document?

I’d love to see a web service that I could send a URL to that would pipe the page through Mozilla and then through [HTML Tidy](http://tidy.sourceforge.net/) and (eventually, presuming this would be a slow process) spit out valid XHTML on the other side.

My secret ulterior motive for all of this is that I want to see people start to work on conferring benefits to sites that use proper XHTML, by offering richer indexing, search, transformation or presentation opportunities. And perhaps the best way to demonstrate these new opportunities on existing, invalid pages would be if we had a way to easily create machine-made valid versions. Granted, the transformations would be imperfect, but they might be close enough to show the potential applications.
