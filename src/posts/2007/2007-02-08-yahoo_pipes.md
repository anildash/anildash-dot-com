---
title: Yahoo Pipes
slug: yahoo_pipes
date_published: 2007-02-08T05:36:09.000Z
date_updated: 2007-02-08T05:36:09.000Z
tags: [Best Of, Most Popular, tech, yahoo]
---

![](http://pipes.yahoo.com/img/logo-lg.gif)**Background:** Yahoo’s launched an interesting and innovative new service, Pipes, which lets users with a relatively low degree of technological expertise combine structured sources of web data such as feeds. In this way, it’s **possible for non-experts to create new web services** for their own use or for public consumption. Pipes combines a remarkably sophisticated development environment with some core social features such as the ability to clone or share the web services you produce. The service is fairly approachable, but somewhat complex once you get just under the surface, and should be moderately successful while radically raising the bar for other tools in its category.

Some quick links if you’re interested in this topic:

- [Plagger](http://plagger.org/): an open-source, installable feed routing system created by Tatsuhiko Miyagawa which performs much of the core functionality of Pipes and is customizable, but lacks the user interface and integrated development environment (IDE) which distinguish Pipes. (Disclaimer, for what it’s worth: I work with Tatsuhiko. But Plagger’s free and not a Six Apart product, so… shrug.)
[![Ain't a Pipe!](http://www.dashes.com/anil/images/ceci-nes-pas-une-pipe.jpg)](http://www.threadless.com/product/543/This_is_not_a_Pipe?streetteam=anildash)
- [Ning](http://www.ning.com/): Perhaps the archetypal social application platform for the web. Headed by Gina Bianchini, Ning has thus far defined the feature set for end-user creation of web applications, though the focus has not been on creating web *services*.
- [An introduction to Unix pipes](http://www.cf.ac.uk/psych/CullingJ/pipes.html). Not merely the inspiration for the name of pipes, the powerful idea of routing data through a series of loosely-connected applications is one of the core concepts that powers most lightweight automation and data processing by non-programmers.
- The Mario-inspired image you see here is available on a [Threadless T-shirt](http://www.threadless.com/product/543/This_is_not_a_Pipe?streetteam=anildash). My wife has one and it is very cute.

### So, what is Pipes?

Okay, with all the introduction out of the way — what the heck is Pipes? Yahoo’s [overview page](http://pipes.yahoo.com/docs/overview) offers the following explanation:

> Pipes is a free online service that lets you remix popular feed types and create data mashups using a visual editor. You can use Pipes to run your own web projects, or publish and share your own web services without ever having to write a line of code.

In practice, this means you can use Pipes to pick a few feeds or APIs to retrieve data from, set up rules for processing the data which is provided by those feeds, prompt for user input in your processing, and then output the processed results as another feed or object format for use in your own applications. In the simplest case, you can apply some straightforward rules to a feed and then subscribe to the end result.
![yahoo-pipes.gif](http://www.dashes.com/anil/images/yahoo-pipes.gif) Pipes also has a full web-based IDE. Even more amazingly, the IDE is incredibly rich and powerful, with the usual complement of editing tools you’d expect from a visual editor in a desktop application. I’d first seen a browser-based IDE for editing [LiveJournal’s S2 style templates](http://www.livejournal.com/customize/advanced/layers.bml), but even that impressive effort pales next to the Pipes IDE. I’ll never learn all of the Pipes IDE’s features, but I will always admire its gee-whizzery.

### Passing the Pipe

Most importantly, and perhaps most key to the success or failure of Pipes, are the social functions that underpin the application. With Pipes, it’s easy to make your own web services public, to clone web services that others have made, or to offer your own services for others to clone. That element of social sharing of code, first pioneered by platforms like Ning, makes the open source ethos much simpler to participate in. Instead of setting up complex version control systems and submitting patches to a central repository, application cloning works on a principal of infinite forking, taking the idea of [embracing failure](http://harvardbusinessonline.hbsp.harvard.edu/hbrsa/en/issue/0702/article/R0702A.jhtml#section19) and building it into the platform. Code ’em all, and let blogs sort ’em out.

There’s also another key accomodation of social functionality: Pipes is *pretty*. As I mentioned in the introduction, much of this type of functionality is technologically possible with tools like Plagger. But, much as I love Plagger, I just don’t have the patience to install half of CPAN to get it running just so I can hand-code an application on top of it. And that’s even though I think it’s a cool idea — imagine if I weren’t already familiar with the concept of routing feeds around.

Pipes is attractive without being overly pretty; There are the requisite nods to Web 2.0 design (it’s blue!), but overall the site is refreshingly straightforward. The IDE is, frankly, a little cluttered unless you’re running on a gigantic monitor, but that’s been true of IDEs since [Visual Studio](http://www.amazon.com/exec/obidos/ASIN/B00005RV4Z/2020-20) was still Visual C++.
![yahoo-pipes-ide.png](http://www.dashes.com/anil/images/yahoo-pipes-ide.png)

### The Bottom Line

Is Pipes going to be a success? **In many ways it already is**. It lets Yahoo unequivocally be *first* at something, and if you count the broader market of web-based application development tools, it lets Yahoo be *best* at something, too. It’s innovative, exciting, and well-done. There are still rough edges and inexplicable nods to the Big Purple Monster. (Whose idea was it to have the Yahoo Messenger anime avatars next to developer names on the site?) But the web needs a way to rip, mix and burn feeds, and Yahoo has stepped up to provide an essential platform in a way that seems open and approachable.

So, [take a look at the docs](http://pipes.yahoo.com/docs/), [browse some pipes](http://pipes.yahoo.com/pipes/), and let me know if any of you can get it hooked up to the firehose that is the [Six Apart Update Stream](http://updates.sixapart.com/) (that’s an endless Atom feed of blog posts, flowing into your pipes at 30 posts a second). Because routing all these streams to the right place is exactly what pipes are for.
