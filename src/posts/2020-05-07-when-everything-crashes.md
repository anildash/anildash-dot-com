---
title: When Every App Crashes
slug: when-everything-crashes
date_published: 2020-05-07T07:34:42.000Z
date_updated: 2020-05-07T07:36:54.000Z
heroimage: https://cdn.glitch.global/c4e475b2-a54e-47e0-973c-ed0bd1b46262/lego-flats.jpeg?v=1669583630904
tags: [tech, culture, web, software]
---

Today, for about half an hour in the afternoon, pretty much every app that you might try on your iPhone would likely have crashed upon opening it. It's probably worth understanding why, but more importantly, worth understanding what that reality *means*. And here, I'm addressing people who aren't coders, aren't engineers, aren't programmers — just regular users of apps.

The flagship mobile apps from Google, Spotify, Apple, NYT, Venmo, Walmart and many other huge companies all broke for about 30 minutes. A simple explanation of the cause is pretty brief: they all use code from Facebook, so when that broke, they all started crashing.

But let's take a deeper look. First, a little context: one surprising thing about programmers is they all regularly, routinely make use of code written by strangers on the internet, often even code written by people who work at competitors. This is the magic of “open source” and it’s kind of amazing. But there’s also a way that companies try to use open source to extend their influence or dominance in the market. In this case, Facebook absolutely wants every app on the internet to use Facebook for login, since that will make both the other companies & their users dependent on Facebook.

For apps, or more specifically for the companies that *create* popular apps, using Facebook login is appealing — users already have an account. Easy! And Facebook made it even easier to take advantage of their billions of logged-in users by writing the code *for* you if you’re a programmer who wants that feature. You can just go get it for free, and plug it into your app pretty quickly and simply. The tricky part, though is that now your app is dependent on that code from Facebook. You have to trust that it works the way they say it will, or you have to read all the code and fully understand it. (That’s almost as much work as just writing the code yourself.) 

So, understandably, everybody just plugs in the Facebook code (often called a “library” or more formally, a Software Development Kit, “SDK”) and focuses on the more important features of their app. But while lots of open source code libraries that you might use just perform a certain function in your app, like displaying a picture or formatting some data, this Facebook code also relies on a service on Facebook’s site running properly, too.

Today, that service got broken.

The result of Facebook's breakdown today is kinda wild: a minor configuration change on a Facebook server that isn’t even visible to regular users made dozens of high-profile apps from some of the biggest companies in the world all start crashing when you open them — even if you weren’t using Facebook at all.

---

## Status: It's Complicated

Done right, open source is magic. It gives coders super powers to build things they could never do alone. But it can also be a strategy that makes huge parts of our online experience dependent on a few companies, and vulnerable to their choices. The failure that millions of people experience today was just (“just”) some apps crashing for a little while. A few weeks ago, it was Zoom using a Facebook library that [sent data](https://www.vice.com/en_us/article/z3b745/zoom-removes-code-that-sends-data-to-facebook) in ways they didn’t disclose. We don’t have a cultural fluency in how to talk about the interconnectedness of all the tech around us.

These issues matter a lot. Our kids are now spending all day connected to apps that use this code. We’ll need to have trusted apps for COVID tracing that *don’t* have these issues — but even if they are done right, many won’t trust them because they’ve learned to be skeptical.

Simply put, we have to demand of our technology what we have of our food, clothing, medicine and other essential needs: visibility into how they’re supplied & sourced, understanding the workers & working conditions that shape them, and accountability when the system has failures. When the supply chain for Tylenol was vulnerable, the manufacturer addressed the issue directly. When consumers wanted to know their tuna was dolphin-safe, companies responded.

That raises a few key questions: **Who makes your apps? Where are they sourced? Which apps do you use that were made by people you trust?**

---

Needless to say, we think about this a lot at [Glitch](https://glitch.com/). Every one of the millions of apps on Glitch was made by a real, regular person. The overwhelming majority have their code clearly visible, and all can be traced to the source project they were remixed from. You can even inspect the history of what was added to the code by remixing an app yourself. And of course the creators are visible right where you see the app — you know everyone who helped make it.

This is an architecture of accountability. It's just one part of a broader ecosystem where millions of creative people around the world are making a more person, more human internet. (In a tech context, we'd call it a "[Yes Code](https://www.linkedin.com/pulse/code-great-heres-why-we-need-yes-anil-dash/)" approach.) While I'm understandably proud of Glitch's role in this kind of work, it's going to take *everyone* making steps toward a world of accountable tech for us to really see wins here. I hope we can teach enough people about these ideas in order to make this a movement that becomes as inevitable as the similar pushes for accountability in other parts of our daily lives.

---

<div class="glitch-embed-wrap" style="height: 420px; width: 100%;">
  <iframe
    src="https://glitch.com/embed/#!/embed/glitter-nails?path=README.md&previewSize=100"
    title="glitter-nails on Glitch"
    allow="geolocation; microphone; camera; midi; vr; encrypted-media"
    style="height: 100%; width: 100%; border: 0;">
  </iframe>
</div>

*glitter nails by Naoto Hieda*
