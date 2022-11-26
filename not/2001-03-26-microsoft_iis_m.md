---
title: Microsoft IIS MetaBase Editing Utility and graceful.bat
slug: microsoft_iis_m
date_published: 2001-03-26T14:22:40.000Z
date_updated: 2001-03-26T14:22:40.000Z
---

Did you know you need the IIS MetaBase [Editing Utility](http://support.microsoft.com/support/kb/articles/Q232/0/68.ASP)? Internet Information Server on NT 4 or Windows 2000 stores all of its configuration info in a little database, similar to the Registry, called the MetaBase. MetaEdit (now in version 2.1) lets you edit the settings.

You still gotta use the [MMC IIS Admin snap-in](http://www.win2000mag.com/Articles/Index.cfm?ArticleID=9159&amp;Key=Microsoft%20Management%20Console%20(MMC)) to back up those settings first, though. Oh, and now might be a good time for me to mention the [batch file I made](__GHOST_URL__/tools/graceful.bat) for IIS, which shuts down the WWW, FTP, and IIS Administration services, in that order, and then starts them back up, in reverse order. It’s called graceful.bat as an homage to the [apachectl graceful switch](http://www.itb.it/apache/docs-2.0/programs/apachectl.html), which does much the same thing.

Yes, this could be done through MMC or other ways, but this way works for me and I love my little batch file. It’s always the second or third thing on the drop-down history list for my "Run…" command.
