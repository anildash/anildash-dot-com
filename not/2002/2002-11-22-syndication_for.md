---
title: syndication formats?
slug: syndication_for
date_published: 2002-11-22T21:23:04.000Z
date_updated: 2002-11-22T21:23:04.000Z
tags: weblogs
---

I have a radical proposal for a ubiqitous content syndication format, applicable for almost any purpose, but extremely well suited for weblogs. It’s extremely simple to implement, either by software or by hand, works already in millions of clients that are very forgiving of misformed or omitted data, and is human readable both in source and output formats. Even better, it doesn’t require any additional work to create the syndication format when creating your website.

My new syndication format is called XHTML. I propose that existing syndication and aggregation clients should be able to read an HTML file, detect if it has the appropriate XHTML [doctype](http://gutfeldt.ch/matthias/articles/doctypeswitch.html), and then render the contents of each XHTML node in the appropriate place in the client’s display. All that would be needed is standardization of names and classes for page elements like DIVs and headers. A post/entry title would always be an H3, with a class set to "title", for example. Permanent links would always be P tags with their classes set to "permalink". Simple.

Content authors shouldn’t have to make two versions of all their content just because people are lazy in the way they make their client software. Valid XHTML *is* a hierarchial outline of content, presented in a machine-parsable manner. Augment this XHTML with proper use of link tags for navigation, and the loss of the page cruft that surrounds the content on a typical HTML page wouldn’t be missed at all. Even better, an [XQuery](http://www.w3.org/TR/xquery/)-based search engine could give you a Google engine that returned relevant *entries* from a site, instead of an entire page, therefore rewarding people who go through the effort by making them participants in a new, better targeted web that’s fully backwards compatible. Existing pages could probably be rewritten by proxies, if the authors are unable or unwilling to reflag their content. Simply iterate through the nodes in the body of the document, find the highest-level node that repeats and contains other content, and you’ve got the pattern that delimits individual entries. Or look for # named anchors that suggest that they’re permalinks. Transform those through XSLT into elements with a predictable set of names.

So, the proposal? A documented standard set of XHTML element names targeted at standardizing class names for page elements, in order to allow HTML to serve as a syndication, aggregation, and distribution format, in addition to being a page rendering format. The side benefit would be that any tool that produced compliant code would probably also be able to share style sheets with other compliant tools, as page elements with the same name would inherit the appropriate styles. A lot easier than forcing tools to output multiple versions of content each time a page is changed. And adaptable to situations like a newspaper, so that articles using the naming convention could also appear in an aggregator.

Rich XML-based descriptions of content are great, and will always have their place. But for something as simple as syndication and distribution, HTML already has an overwhelming advantage over any nascent formats. Who wants to propose a set of basic tags?
