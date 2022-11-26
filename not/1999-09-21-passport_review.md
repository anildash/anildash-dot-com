---
title: Passport Review
slug: passport_review
date_published: 1999-09-21T16:00:01.000Z
date_updated: 1999-09-21T16:00:01.000Z
tags: tech
---

As promised:

![Microsoft Passport](images/mspass.gif)

### Microsoft Passport Part One: User Experience

Okay, so after spending waaaay too much time reading all the documentation at the official Passport site, I’ve been able to glean a little info on how the end-user will approach this technology.

This analysis is necessarily focused on the **Wallet** component of Passport, because this component (1) **doesn’t require NT** Server’s IIS, which I don’t use, (2) can be **referenced from any site** through standard protocols, making its adoption much more likely to be pervasive, and (3) is **closer to a release** product. Enough intro, though, let’s see what we’ve got…

First, let’s address the **goals**, as I understand them:

**Reduce duplicate data entry of personal information:** Great one, very needed, and relatively well addressed. The only clear win with Passport.

**Increase security of info:** Another essential. Remains to be seen how well this one is handled, but Microsoft has a checkered history in this area, especially after the recent Hotmail CGI vulnerability.

**Introduces consistent e-commerce interface:** Mixed bag. Consistency *between* multiple commerce sites **reduces** consistency *within* an individual site, assuming sites have significantly different designs, as most do. (see below)

An unstated, but likely, goal: **Increasing the number of sites using secure technologies for transactions and registration:** Will very likely succeed in this area, but adoption rates are notoriously hard to predict on the web.

**Increase user comfort:** Remains to be seen. Seeing Microsoft’s name should comfort most users, except possibly Linux users. The strength/weakness of the system is that all Password sites reinforce each others’ images of security or vulnerability.

### ![Passport](images/passport.gif)    Whipping Out Your Passport

Let’s go deeper into this. The fundamental thing to know about Passport is that it’s a **typical Microsoft web initiative**, equal parts evangelism, assimilation, marketing, and technology. That being said, it also displays Microsoft’s usual knack for *eventually* resulting in end-user benefits by **shamelessly pandering to developers**.

Users (and in this context, I mean end-users on their web browsers at home on a dial-up) browse to your site. You’ve got your **special features**: a "Members Only" section with proprietary content, a little Shopping Cart e-boutique selling your logo gear, and your usual bevy of doodads, the site search, your homepage, the ugly slow page your client made you lard on despite your objections.

User X is new to your site, but desperately wants to see that [New York Times](http://www.nytimes.com)-style "Registration Required" material. So they click on the standard **Passport Sign In Icon** on your page.

![Passport Sign In](images/passsignin.gif)

Your server talks to Microsoft’s, and they work out all the details. (More on the tech stuff tomorrow) **We’re in luck!** User X has a Hotmail account already, so they’re spared the ritual of registering for Passport. (Which isn’t very trying, anyway.)

X sees the "standard" Passport sign in screen, and this is **where the trouble starts**.

**Coming up:** an in-depth look at [Microsoft Passport](http://www.passport.com). Until I get all of that uploaded, take a look around their website and give me some [feedback](mailto:anil@dashes.com) of your own.

Specifically, part one today will deal with **user experience** and part two tomorrow will describe the (rather ungainly) **back-end technology** that makes it work from the site manager’s perspective.

**Note:** Much of the information on the Passport site requires that you already *have* a passport, which you do if you have a [Hotmail](http://www.hotmail.com) account.

While the [list of sites using Passport](http://www.passport.com/directory.asp) right now is very short and limited to [MSN](http://www.msn.com) sites, I’m expecting we’ll see more of this technology (and, presumably, the inevitable open-source alternative) all over the web soon. Stay tuned…
