---
title: Web Development Trends for 2006
slug: web_development_trends_for_200
date_published: 2005-09-07T02:55:07.000Z
date_updated: 2021-12-23T23:30:34.000Z
tags: Best Of, Most Popular, tech
---

Curious about what technologies and techniques are going to be popular in the coming months and into the next year? Well, our crack team of editors here at dashes.com (that is to say, me) have assembled a list of up-and-coming trends that you should keep an eye on. Call it vocational education for people building Web 2.0.

Some of the overall areas of focus are integration (as always) and front-end technologies that have highly visible impacts on end user experience. People won’t pay for a service or rely on it if it doesn’t have a robust back-end infrastructure, but they’ll be happy to pay for it if the front-end is attractive and at least *seems* usable.

Here, then, is a random assortment of new web development trends to be ready for in 2006.

- **Dampening:**

These technologies go by a lot of names, but in general, dampening is the softening of a user interface through gradual transition instead of immediate state changes. The demand for dampening reflects the front-end focus that is being rediscovered in web applications, but it can require server-side changes in order to enable some effects. The best-marketed example of dampening is the [yellow fade technique](http://www.37signals.com/svn/archives/000558.php), but overall, user interface elements will be sliding and collapsing instead of simply disappearing.

Key influences on the user experience here are things like the iPod screen backlight fading out instead of merely shutting off, or soft-close doors on newer automobiles.
- **E4X:**

This [little-known ECMA standard](http://www.ecma-international.org/publications/standards/Ecma-357.htm) is short for “ECMAscript for XML”. That mouthful succinctly describes a powerful concept: Smart, sensible handling of XML in Javascript. Right now, the J and the X in Ajax don’t play well together, or at least not as well as they should. [E4X](http://en.wikipedia.org/wiki/E4X) promises to smooth that combination, at least in more modern/capable user agents. Support is already present, or will soon be, in both the Flash player and Firefox.

What’s the quick synopsis? How ’bout building a form dynamically by doing this:

    var html = 
    ; html.head.title = "Hello, World."; html.body.form.@name = "hello"; html.body.form.@action = "test.php"; html.body.form.@method = "post"; html.body.form.@onclick = "return foo();"; html.body.form.input[0] = ""; html.body.form.input[0].@name = "Submit";
    

- **JSON:**

Why will you want to use [JSON](http://www.crockford.com/JSON/index.html) to send the data your application is managing? Broad language support. It’s simple to read and write. It’s designed for transporting structs in a manner that your programming language is used to. And despite the comparisons, don’t let anyone frame it as an us vs. them thing: It’s just a smart way to handle your data, and it works well with XML: you can just transform to/from XML when needed. There’s even a [JSON-RPC](http://json-rpc.org/) if you’re so inclined.
- Good ole’ **XHTML and CSS:**

Call me old-fashioned, but the basics are always in style. *Plenty* of sites still haven’t had the time, resources, or education to move to standards-based design, but even fewer applications have made the move. Just as many corporate sites relaunched with valid markup, many web apps for intranets or public consumption will be restyling themselves with well-matched tags. In a Greasemonkey-enabled web, it’s going to be more important than ever to have a reliable structure that you can hang new behaviors on.
- **Buffering:**

Just like dampening, this is a return of an old favorite desktop application technique, but (re-)inflicted on the web. Users who’ve just gotten past seeing the “Buffering…” message in RealPlayer or who are tired of watching “Loading…” graphics on the sites that still abuse Flash for skipped intros will be encountering the same “Please Wait” experience again. But this time, it’s the advanced behaviors and Javascripts that power their Ajax apps that will have them twiddling their thumbs. Progressive enhancement isn’t just about adding behaviors or presentation to only the user agents that support them, it’s about offering a useful experience in full-featured browsers even while the oodles of script are still loading.

Let people get to work quicker, even while the whizzy stuff is loading in the background, and you’ll never be accused of forgetting that half the people on the web in the United States are still on dial-up.
- **The Atom API:**

The fuss (and flamewars) were always over the feed format, but the interesting part of Atom has always been the API, or the Atom Publishing Protocol, if you want to be formal. Now that the feed format is an IETF standard, there’s a solid enough spec to start planning for how the API will be built on that core. And with over twenty million blogs already supporting pre-release versions of the spec, it’s extremely likely that investing in familiarity with the API now will give you a heads-up in 2006. Pretty much everyone will be clamoring for their applications to connect to blogs via Atom as it gets added to the standards-compliance checklist.
- **Helping Ruby Grow Up:**

Everybody loves Ruby on Rails, except those who think it’s overhyped. Regardless of where you stand on the best-since-sliced-bread/kills-puppies-for-breakfast continuum, there’s a lot of development and even deployment happening on the Ruby platform. But key parts of the infrastructure are missing. Localization? Internationalization? They’re a f18king pain. Scaling up servers to handle *really* large applications or high-demand situations? Nobody’s really done that at a global scale yet. Interop with other languages? Aside from the “it’s all just XML!” form of interoperability, there’s a lot of unsolved problems here.

While everyone else is just learning the language and oohing and aahing over the elegance of the framework, you can be digging into the hard problems *behind* the applications and take advantage of a wide-open opportunity.

- **Marketing:**

Okay, this one’s not a technology. But geeks *really* need to learn how to explain their skills, the benefits of their skills, and the business advantages provided by those benefits. Knowing half a dozen programming languages won’t help you if you can’t communicate with the people who want to hire you. And your language/platform/development environment of choice won’t succeed unless you do a great job of evangelizing it and promoting it to others, including non-technical people.

First, be an expert with a technology. Second, be even better at explaining the value of that technology. If you can do those things, it doesn’t matter which of the items you pick off of the list above.

### The Bottom Line

If you have a friend who’s looking to change jobs, or know a disgruntled person who’s been laid off and Lou Dobbs has convinced him to blame Indian engineers for it, send them this list, and check back with them in a few months to see if they’ve taken the time to learn some new skills. No whining, just go do some reading. Buy some O’Reilly books or Google up some docs online, and then get hacking. By the time you’re good enough to start posting your sample applications, employers will be searching for your blog just to find the talent they need.

Got more ideas of what should we should be studying up on? Feel free to comment.
