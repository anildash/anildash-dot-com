---
title: danger revisited
slug: danger_revisite
date_published: 2002-10-10T04:10:57.000Z
date_updated: 2002-10-10T04:10:57.000Z
tags: tech
---

I realized sometime on Monday that it was gonna happen. Too many people reading it, the Network Effect had been triggered, and I was expecting an email any minute. Sure enough, I got an email from a web app engineer at Danger, in response to [my rantings](http://www.dashes.com/anil/index.php?archives/003378.php) the other day. Her message said:

> I was entertained by your October 3 rant on how the hiptop mangles your web page. I’ve forwarded the link to our web proxy team — I’m sure they’ll appreciate the feedback. I apologize for my ignorance as to the inner workings of your web site, but do you have any specific examples as to how we “took it upon [ourselves] to write software to specifically fuck up [your] website’s display on [our] device”? Is it a CSS problem? I just want to be able to give as much info to our proxy people as possible. I doubt we intentionally wrote software to fuck up your page, but knowing our web proxy team, anything’s possible… 😉

Well-mannered, funny, and kind. That’s *no* way to respond to an obscenity-laced rant! Sigh. So of course, I had to reply:

> Ya know, I was fearing this email. Now I feel bad, because these rants always lead to me giving people the impression that I was *actually* angry. Heh. I’m actually very sympathetic to what your engineers have to do to make sites look and function appropriately within the constraints and limitations of the device, especially given that it’s upgradeable and can only improve.

> That being said, the problem with the browser client on the HipTop is that CSS is designed to specify appearance for a certain target audience. Most commonly, people use the “screen” media type for styles, and a few set “print” media types if they want to specify a layout for print output. There is, however, a “handheld” media type, and a literate version of my screed would have called for adherence to CSS settings authored for that audience.

> Media types are described here: [W3C](http://www.w3.org/TR/REC-CSS2/media.html)

> Meanwhile, back in the real world, nobody uses CSS media types at all. Let alone to create handheld-specific versions of their style sheets. But a good compromise would be what the desktop browser manufacturers call “quirks mode”. If a page is designed to comply with standards, by indicating the type of HTML with a statement at the top of the page, then the HipTop/Sidekick could obey the CSS rules as the media type dictates. Else, you could still try interpreting screen designs for the handheld, as you’re doing now.

> Quirks mode description here: [doctype info](http://gutfeldt.ch/matthias/articles/doctypeswitch.html)

> At any rate, I do understand what a tough problem it is to solve, and I appreciate you having a sense of humor about my rantings. Chalk it up as a tribute to your development and marketing teams that even people who don’t own the device can be passionate enough about it to express their disappointment or frustration with such vehemence. Let me know if your dev staff wants any other info. I can’t give them any specifics on the display of my particular page, as I don’t actually *own* the device. But I’d be glad to give them my perspectives on ways to more gracefully degrade the display of web pages through the proxy.

After I wrote the email, I saw that Scott had covered much of the same ground over at the [Web Standards Project](http://www.webstandards.org/buzz/archive/2002_10.html#a000092).
