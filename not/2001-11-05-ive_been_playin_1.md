---
title: I've been playing around with
slug: ive_been_playin_1
date_published: 2001-11-05T08:12:16.000Z
date_updated: 2001-11-05T08:12:16.000Z
---

I’ve been playing around with making a totally desaturated version of the default blue theme that ships as part of the updated UI in Windows XP. This idea has been haunting me since the first betas shipped with the new interface, as any time a user changes themes or logs off the system, the system slowly fades the desktop and all open apps into a very nice grayscale display. It’s subtle and, in a big departure for Microsoft, **actually quite elegant**. Needless to say, since it’s a chance at making Windows more elegant, there’s no way to make your normal interface look like that. Yet.

But, as part of my playing around with the theme features, I thought I should offer you a little XML file that I made a while ago. Right now, its name is [Photoshp.exe.manifest](http://www.dashes.com/tools/Photoshp.exe.manifest). Right-click on that link and choose “Save to Desktop” to grab the file. As the name suggests, I made this file to be placed into your Photoshop directory. (Which is usually \Program Files\Adobe\Photoshop 6.0\ or something like that.) Its effects in Photoshop are subtle, though, so you may want to rename it to the same name as any other .exe on your system, and then drop it into the appropriate folder for your program.

What is the file? It’s an XML manifest, telling Windows XP that your program uses the common controls for the display of UI widgets, and that they should be rendered in whatever theme you have selected, instead of just defaulting to the old ones built into the program. **Is that useful? No, not particularly.** But it is a way to make the interface in all of your applications a little more consistent. And I think it’s damned cool that a 665 byte text file can affect the appearance of these huge old programs.
