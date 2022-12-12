---
title: mac html control suckage
slug: mac_html_contro
date_published: 2002-10-20T07:09:00.000Z
date_updated: 2002-10-20T07:09:00.000Z
tags: tech
---

You heard it here first: Internet Explorer for the Macintosh is the new Netscape 4.

On a more substantive Macintosh web development note, we know that OS X shipped with a [Text View control](http://developer.apple.com/techpubs/macosx/Cocoa/TasksAndConcepts/ProgrammingTopics/UITextView/index.html) that, while undocumented, is able to render HTML like a primitive browser. At least, I *think* that’s what [Brent’s referring to](http://ranchero.com/software/netnewswire/faq.php#htmlpane) as the "system’s built-in HTML renderer". But it seems to me that it’s a foolish bit of duplicate development on Apple’s part, especially as the HTML renderer is apparently so crippled. Why not follow a tack similar to [last week’s scripting engine suggestions](http://www.dashes.com/anil/index.php?archives/003545.php) and embed Mozilla’s Gecko engine as the system-level HTML rendering control in OS X?

I know that’s perilously close to (*egads!*) bundling a browser engine and then hiding access to it, but it’d make the Mac that much more more credible a development platform. Most Mac users don’t realize just how many Windows applications, even non-Microsoft ones, embed the Internet Explorer control to display HTML in all of the many places that such funcionality is useful. Mac users are sorely missing out on these opportunities, especially since they could be offered without the security risks of Internet Explorer and could be integrated with AppleScript.

That is, unless the Mac IE team has been busy making their browser embeddable in Mac apps, and that’s why their next release is taking so damn long to come out.

**Update:** Brent points out that OS X’s HTML rendering [is documented](http://developer.apple.com/techpubs/macosx/Cocoa/Reference/ApplicationKit/ObjC_classic/Classes/NSAttributedString.html#//apple_ref/occ/instm/NSAttributedString/initWithHTML:documentAttributes:), and that Apple did recently hire [David Hyatt](http://www.mozillazine.org/weblogs/hyatt/2002_07_14_mozillian_archive.html), creator of [Chimera](http://chimera.mozdev.org), so maybe they’re progressing on this topic yet.
