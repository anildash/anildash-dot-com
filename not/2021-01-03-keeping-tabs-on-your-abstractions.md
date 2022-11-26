---
title: Keeping Tabs on your Abstractions
slug: keeping-tabs-on-your-abstractions
date_published: 2021-01-03T09:48:45.000Z
date_updated: 2021-01-03T14:20:46.000Z
---

I was delighted to discover Omar Rizwan's [TabFS](https://omar.website/tabfs/), a brilliant hack that lets you see your browser tabs as folders and files on your computer, because it's incredibly clever on its own, but also opens a view into how a shift in metaphor  can totally change the way we see technologies that we use every day.

On its own, TabFS lets us apply an entire mature, flourishing ecosystem of tools — the ones we use to manage and manipulate files on our computers — to a new domain that has almost *no* effective management tools: our unruly web browser tabs. In his writeup of TabFS, Omar casually throws out the following mind-bomb:

> there are two 'operating systems' on my computer, the browser and Unix, and Unix is by far the more accessible and programmable and cohesive as a computing environment (it has concepts that compose! shell, processes, files), even though it's arguably the less important to my daily life.

Almost everyone goes through two steps when they hear about TabFS. First, there's a bit of struggling to understand the concept, and an initial dismissal or head-shaking. Then, the amazing thing happens: almost *anyone* can think of something they would do with TabFS. It's easy to imagine this early, rough demonstration being productized into something any ordinary user could find value in. We can picture an experience your web browser folder just becomes part of your computer in the same way that your Dropbox folder did, with the same radical increase in capability through a vast simplification of a formerly-complex process.

### What Meta is For

This is the power of good metaphors in technology. While many abstractions just add complexity or new points of failure, every once in a while, exposing one system so that it resembles another upgrades everyone's brains and makes new things possible. Unix famously did this with processes, making a file system a consistent interface for things that aren't files, and in doing so, revealing that these mental models are as flexible as we choose to make them.

I'd seen this a bit in our work at [Glitch](https://glitch.com/), when we introduced [Rewind](https://medium.com/glitch/reinventing-version-control-with-glitch-rewind-914c350da442) as a new interface for version control. Put simply, we used the same timeline metaphor that you use to rewind a YouTube video or to scroll through a media clip in editing software, and applied it to git code commits that are typically displayed as a list. By refocusing the interface to focus on progress over time, instead of a list of actions in which any given item might be massive or trivial, we help communicate a completely different mental model than most people are used to facing with these kinds of collaboration. New metaphors are powerful; GitHub's homepage now uses the word "rewind" to describe their version control system even though it still features the same text-based list interface it always has. Even those who haven't adopted the improved user experince can reflexively see how the new mental model provided by this metaphor can help people understand a complex concept.

    Sorry, your browser doesn't support embedded videos.

And the same goes for TabFS. What it shows us is that tabs aren't *just* a tool for managing individual pages in a web browser app. As Rusty Foster shows us (hey, [Today in Tabs](https://www.todayintabs.com/) is back!), "tabs" can be a metaphor for the role that content plays in our lives, a shorthand way of saying media or content or hot takes. And what Omar's work shows us is that tabs are every bit as important to us as any individual app on our phones, or any particular document that we've created. Suddenly, we realize that not being able to actively manage and orchestrate tabs is an egregious shortcoming. How is it that the only thing we've been able to do with a tab is to file it away as a bookmark that we'll never revisit?

Now, the floodgates are open. Aside from an easier install process, the immediate feature request I had for tabs hackers is that any text-editing area in a web page (like the one I'm using to write this blog post!) should be presented as a text file within that tab's folder on my computer. Then, we don't have to do complex gymnastics to shoehorn a text editor into the web browser — I can just use the text editor I've already got on my machine.

From there, the sky's the limit. What about a tab history interface that looks like the Time Machine interface I use to restore file backups? With Glitch, we've found that people being able to instantly edit a live web app in their web browser changes the kinds of apps they make — lowering barriers and increasing immediacy makes things more expressive and makes people more willing to try new things out. TabFS promises to introduce that same kind of experimentation and whimsy to the dozens of tabs we all have open every day, and perhaps to reveal to a new audience that what's felt like "browsing the web" for the last 3 decades is, also, simply a really good interface for transferring some files from a distant computer to a closer computer. 

What will we discover just by being shown a different metaphor for what we've been doing all along?
