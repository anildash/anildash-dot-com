---
title: IE scripting engines
slug: ie_scripting_en
date_published: 2002-10-17T01:45:33.000Z
date_updated: 2002-10-17T01:45:33.000Z
tags: tech
---

Internet Explorer for Windows was designed to accept multiple scripting engines to interact with HTML documents that it renders. The system for integrating these languages was a vestige from the days when everything from Microsoft was Active or Direct, instead of being .NET, so they were labeled Active Scripting languages. IE ships with two: JScript, Microsoft’s implementation of JavaScript/ECMAScript, and VBScript, based on the syntax of Visual Basic.

Since then, the Active Scripting languages became general purpose-scripting languages for automating general functions in Windows, much to the delight of system administrators and virus authors. They were also used in creating Active Server Pages. But people forgot along the line that they were modular and extensible, except in the "you can disable them for security’s sake" sense.

So. I propose that somebody (You, maybe? Not me, I’m lazy.) create a new implementation of ECMAScript as an Active Scripting language, perhaps by leveraging some of the code from Mozilla. Except, in this IE scripting language, you’d be able to disable individual events, or modify how they fire.

The benefit? Lots of things. You could, of course, disable the firing of the window.open command from within the onload or onunload events of the page, thereby killing popups in the same elegant, effective, and appropriate manner that Mozilla does. But there’s probably a lot more you could do by giving the huge user base of IE/Win users this flexibility. And you’d have the only scripting language that would have a user base that included end users in addition to developers. Bonus.

Get to it, kids!
