---
title: Stories and Tools
slug: stories_and_too
date_published: 2002-04-09T07:00:59.000Z
date_updated: 2002-04-09T07:00:59.000Z
tags: Best Of, magazine, tech, Most Popular
---

The current world wide web consists almost entirely of pages that are either stories or tools. A few ambitious sites combine these two types of web pages in varying ratios, with results that range from unsatisfying to disastrous. But I asserted [a few days ago](http://www.dashes.com/anil/2002/04/03/next_web) that the next stage of the web is going to come from the native form that evolves from, and incorporates elements of, these two existing structures. Even after this form emerges, however, the web will still be populated with plenty of stories and tools, of course, just as television retained the idiom of an anchor at a desk authoritatively reading us the news, even after the invention of the situation comedy and the game show.

If you take a look at the pages we have today, one thing becomes clear: **Stories on the web just plain work**. The obvious, and so far ultimate, display of this is [The Fray](http://fray.com), of course, which sets out in its very mission to tell stories. It’s the definitive example. But less obvious examples are abundant and instructive. Every news item proffered on whatever portal or provider you prefer is presenting a story. The content presented in web interfaces to [Usenet](http://groups.google.com) and [email](http://hotmail.com) are largely story-oriented. In a medium originally designed to [present structured documents](http://www.w3.org/People/Berners-Lee/WorldWideWeb.html), the natural divisions and regular formatting of stories was destined to be a good fit, even if they technically fell outside the precise realm envisioned by the web’s creator.

This brings us to the other kind of web page, the kind that just plain *doesn’t fit* into how the web was envisioned: tools. Web pages that aren’t stories are tools that you use to perform a task. You’ve probably seen these. Amazon is one. Your bank’s online payment system is another. You probably use a web email tool like Hotmail. This site’s been using Blogger for a few years now. Hell, Yahoo, MSN, Netscape, and most other common start pages are more tools than story already. **And none of them work right.**

That’s not surprising; they’re not supposed to.

Think of Hotmail. It’s designed to give you a place to write emails, read them, and move them into folders. These kinds of functions in a desktop program like the Mac Finder or the Windows Explorer are automatic. You just drag and drop. But to enable that kind of ability in a web page, programmers have to jump through hoops, trying to make a story act like a tool.

And notice who has to do that? *Programmers*. But HTML isn’t a programming language. And it’s designed to be written by *authors*, not programmers. There are tags to describe the parts of a structured story. There’s in fact a formal Document Type Description for hierarchially structured documents, that’s what XHTML is. Curiously absent, unfortunately, is a description for a Web Tool Document.

Look at [Oddpost](http://oddpost.com), as it’s been making the rounds lately. It solves most of the problem. It’s beautiful, useful, powerful. And, much to the chagrin of Mac partisans and Unix enthusiasts, it only works on recent Microsoft browsers on Windows. That’s not the bad part about Oddpost, though, that’s just smart use of limited development resources. What’s truly bad is that Oddpost’s HTML doesn’t make any sense outside of a very limited context, and it’s incredibly hard to debug or reuse or make useful on a PDA or a non-standard web platform.

It was this opening that [Flash MX](http://news.com.com/2100-1001-872136.html) stepped into. With a cry of anguish from standards and open-source advocates, and amidst shouts of glee from newly-empowered Flash developers, Macromedia recognized the enormous opportunity to make tools easy to build. And if it just so happens that most of the money in the web development business comes from helping businesses build tools, not from helping businesses tell stories, well that’s just plain old good luck for Macromedia. And it was an inevitable opportunity because the web was always, and only, designed to be stories. All else is kludge.

### A Way Out?

What was needed was a formal DTD for describing elements of a web-based application. Common GUI widgets like a tree control, a select or combo list, a spinner control, some drop-down menu controls, toolbar buttons, scrollbars, and all the other usual trappings of a modern GUI application. And some basic logic for loops and form processing. This Application Markup Language would just be a specific XML implementation, with the unique part being that all of the controls would be rendered as GUI-native, state-aware *real* widgets. But these HTML applications would still have all the benefits of web applications, as benefits like CSS styling, device-neutral rendering, and simple data sourcing would be preserved.

Thus was born [AppML](http://www.w3schools.com/appml/). It’s beautiful, really. But nobody’s using it. And it requires server-side logic to execute. And it only exists in theory; I couldn’t build Oddpost with it in any reasonable amount of time or under any reasonable budget.

Does that mean we have to give up? The choice is shitty apps or an extension of Microsoft’s hegemony? (For the record, I don’t think that idea’s nearly as evil as an extension of the tyranny of desktop applications and humongous computer form factors.) Well, no. I think there’s a third way.

A widely-distributed, standards-compliant, browser and platform-independent library of functions that would perform the basic user interface functions for a web-based tool, relying on the server side only for the logic and data sourcing. Well, whadaya know? [We’ve got one](http://domapi.com). Yeah, it’s still a work in progress, and it doesn’t support nearly enough platforms yet. But DOMAPI is spectacular already. And it’ll evolve, and it’ll be [good enough](http://www.jwz.org/doc/worse-is-better.html) a year from now to be the basis of a large, stable array of applications, guaranteeing its future development and viability.

So what does all this mean? It means that we’ve finally got something that works for the two main uses of today’s web. We can stop fretting and take these two essential pillars of the future web for granted. Stories we’ve got beat. Applications we’ve got a little distance to travel yet. But now… now, we’re ready to figure out what the web will actually be used for.

Have we *really* almost finished writing the first chapter of the web’s history?
