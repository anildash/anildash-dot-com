---
title: blogger gets hacked
slug: blogger_gets_ha
date_published: 2002-10-25T15:21:00.000Z
date_updated: 2002-10-25T15:21:00.000Z
tags: weblogs
---

### Post-Hack Update

Blogger’s completely [back up](http://status.blogger.com), including bStats and the API. It seems (again, I don’t work for Pyra, but I’ve had information confirmed by Ev) that the vulnerability was was really only severe during the hour or so that Blogger was running while hacked. During that time, it was possible, if you knew another user’s login name, to use the “hacxoredbyme” password and post and publish with any other user’s account.

It does not seem, at any time, that *anyone*, including the hacker, could read the server passwords in the system. In technical parlance, the intruder had “update” privileges on the system that stored less sensitive information like the public URL of the site, but no “select” privileges on any database, including the separate one that stores sensitive things like users’ server login name and password.

In short, (s)he couldn’t even read the database that was screwed up, let alone the other one that had sensitive data.

All of this is information that I’m not 100% positive is correct, but that I’m willing to stand behind as *probably* right. There are hacks that are so well-engineered that a visible hack like the one I reported on yesterday is all a diversion from some other activities that are masked by the part that gets attention. Neither the Pyra folks nor I (for what that’s worth, I’m no expert on this part of it) think this intruder was that sophisticated.

Blogger is, now, at exactly the same security level it was two days ago, minus the vulnerability that caused this hack. Your sensitive information (by that, I don’t mean things like your public URL) is no more or less vulnerable than it’s always been. You can use your feelings about that to decide what information, if any, you should change regarding your server, and whether you want to use Blogger’s feature that lets you store your password.

For all the Slashdot readers who were revelling at Blogger’s misfortune because the blogger.com domain runs on Microsoft’s IIS: the server database which was compromised was attacked through a known, but unpatched, vulnerability on the operating system on which it was running. That operating system is Red Hat Linux, proving once again that the keys to security are meticulous discipline in keeping updated on information, removing unnecessary services, and designing and launching applications with security in mind.

Finally, Ev told me that he intends to be more proactive in communicating with customers in the future. I think that’s the best thing he can do to restore trust in his company and product.

### Original announcement

Any of you who use [Blogger](http://www.blogger.com) will want to log in right now (if you can) and delete your server information and passwords. It looks like a hack is in progress that first switched many users’ passwords or server information to “hacx0redbyme” or “hax0redbyme” and is now prohibiting lots of users from logging in. [Tom](http://www.plasticbag.org) pointed the problem out to me, and at that point it was mostly Pro users having problems, although it seems to be everyone now.

**Update:** Blogger’s now offline, and the problem’s being worked on.

### Some Lessons

I wanted to address some of the concerns people have brought up about its security. Some have suggested that this is an issue because of the design of Blogger’s service, and that decentralization is the solution. I think we’ve seen that decentralization isn’t necessarily a panacea. (Greymatter had a serious security hole; Installations of Outlook and Exchange are decentralized.) The greater issue is reliability and whether weblogging can get out of its mindset of being a hobby and an amateur effort.

Development right now is usually done like kids hacking on a project, where staying up all night and then flipping a switch where something goes live is considered acceptable practice. That’s only ever going to result in insecurity over the long run. It’s even more unacceptable when in charge of a database that probably has the world’s largest collection of server logins.

That’s not meant as a slight to anyone who builds blogging tools, as I was the [first public user](http://www.dashes.com/anil/index.php?archives/001313.php) in the directory and used Blogger for years and was overall very happy with it. But, with the exception of Mena and Ben Trott’s work on [Movable Type](http://www.movabletype.org), which has been informed by Ben’s background in cryptography and other security practices, there hasn’t been a seriousness about the responsibility of developing these applications as weblogs move to being a critical communication tool for people. This is one of the reasons that weblogs aren’t generally taken seriously as business tools.

I recently mentioned, to someone less familiar with weblogs, that the process of writing a weblog with a tool as being similar using Hotmail, except you’re sending your message to people whom you don’t yet know. Unfortunate security parallels aside, one of the lessons of that parallel is that these are tools that people depend on, and they have to be developed and maintained with the seriousness that responsibility entails.
