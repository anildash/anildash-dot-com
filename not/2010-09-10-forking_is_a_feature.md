---
title: Forking is a Feature
slug: forking_is_a_feature
date_published: 2010-09-10T22:03:00.000Z
date_updated: 2018-05-18T18:04:09.000Z
tags: Most Popular
---

While Linus Torvalds is best known as the creator of Linux, it’s one of his more geeky creations, and the social implications of its design, that may well end up being his greatest legacy. Because Linus has, in just a few short years, changed the social dynamic around forking, turning the idea of multiple versions of a work from a cultural weakness into a cultural strength.

Perhaps the technologies that let us easily collaborate together online have finally matured enough to let our work reflect the reality that some problems are better solved with lots of different efforts instead of one committee-built compromise.
![GitHub's map of code forks](https://web.archive.org/web/20110122123626if_/http://dashes.com/anil/images/github-fork-map.png)

The idea of “open source” in the technology world is really a set of cultural beliefs, despite usually masquerading as technical or legal choices made by a community. All cultures have norms, and standards of behavior, and most importantly, they have behaviors they consider antisocial or destructive.

For most of the first three decades of open source’s ascendance, the most destructive action that one could threaten to do, the nuclear option, was to fork.

### Tuning

There are several related technical concepts that can answer to the name “fork”, but the one I reference here is the dramatic moment when a software project undergoes a schism on ideological or technical grounds. Instead of merely taking their ball and going home, those who forked were taking a copy of your ball and going to a new playground. And while splitting a community could obviously cause an open source community’s momentum to grind to a halt, even the mere *threat* of a fork could cause significant problems, by revealing conflicting goals or desires or motivations within a previously-united community.

Still, forks have had important consequences. Firefox (earlier [Firebird](__GHOST_URL__/2003/07/upon-the-demise.html) and Phoenix) was originally a fork of Mozilla, the open source browser that had been mired in indecision for half a decade. WordPress was born as a fork of B2, a neglected early blogging tool.

Outside of tech, forks have an even bigger meaning. You could make a pretty strong argument that the Reformation was a fork, or that Christianity itself is a fork. So clearly, forking a community can have a significant, even profound impact. But in tech, it had largely been seen solely as a violent, schismatic action.

Part of the predicate for forks being so disruptive was the idea that there is One True Version — a creation, like a piece of software, a written work, or anything else, that can only be accurately represented by a single ideal expression. Even some of the most disruptive technological innovations like Wikipedia are still built around the idea of achieving consensus on a definitive work, and striving mightily to avoid forks arising within the community.

Until a git named Linus changed that.

### In The Road

You know Linus Torvalds, he’s the guy who created (and nearly eponymized) Linux. But perhaps his *most* impressive act of creating technological culture is in fathering Git, the enormously popular distributed revision control system. That mouthful of a description basically means “system that lets a decentralized group of creators efficiently collaborate on a complicated bit of software”. Other systems had enabled distributed revision control before, making it easier to rapidly evolve software, and to appropriately assign blame to whomever had introduced a bug into the program, but few had found any notable degree of popularity.
![Forking on GitHub](https://web.archive.org/web/20101112120955if_/http://dashes.com/anil/images/github-fork.png)

But Linus’ pedigree, influence and outstanding implementation immediately put Git at the forefront of choices to solve this class of problem. Even better, his credibility with the new generation of social software creators inspired the rapid launch and brilliant evolution of [GitHub](http://github.com/), a social network for developers that relies on the technology of Git as its underpinnings, but has also embraced the *philosophy* of Git as its fundamental interaction model.

Often, the very *first* thing a coder does when she sees an interesting new project on GitHub is to make a fork of it and start tinkering. That’s only one of the reasons that GitHub so important, though; The GitHub principle of “see it, make your own version, and then get to work” has started to filter into other disciplines, as exemplified by design sites like [Dribbble](http://dribbble.com/), and upcoming new sites for creatives such as [Forrst](http://forrst.com/).

These new sites are admittedly still in their formative stages — Dribbble just had its breakout moment with the recent popularity of redesigning the iTunes icon — but it’s easy to imagine a more mature version where, instead of merely focusing on the pretty pixels on the screen, the designers who frequent the site were encouraged to describe their rationale, and to use the site’s replying abilities (called “rebounds”on Dribbble) to do something more akin to forking, where raw Photoshop and Illustrator files were shared.

### The One True Version

Most importantly, the new culture of ubiquitous forking can have profound impacts on lots of other categories of software. There have been recent rumblings that participation in Wikipedia editing has plateaued, or even begun to decline. Aside from the (frankly, absurd) idea that “everything’s already been documented!” one of the best ways for Wikipedia to reinvigorate itself, and to break away from the stultifying and arcane editing discussions that are its worst feature, could be to embrace the idea that there’s not One True Version of every Wikipedia article.

A new-generation Wikipedia based on Git-style technologies could allow there to be not just one [Ocelot](http://en.wikipedia.org/wiki/Ocelot) article per language, but an infinite number of them, each of which could be easily mixed and merged into your own preferred version. Wikipedia already technically has similar abilities on the back end, of course, but the software’s cultural bias is still towards producing a definitive consensus version instead of seeing multiple variations as beneficial.

There are plenty of other cultural predecessors for the idea of forking, all demonstrating that moving away from the need for a forced consensus can be great for innovation, while also reducing social tensions. Our work on [ThinkUp](http://github.com/ginatrapani/ThinkUp) at [Expert Labs](http://expertlabs.org/) has seen a tremendous increase in programmers participating, without any of the usual flame wars or antagonism that frequently pop up on open source mailing lists. Some part of that is attributable to the cultural infrastructure GitHub provides for participation.

Moving forward, there are a lot more lessons we can learn if we build our social tools with the assumption that no one version of any document, app, or narrative needs to be the definitive one. We might even make our software, and our communities, more inclusive if we embrace the forking ourselves.
