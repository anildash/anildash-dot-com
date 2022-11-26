---
title: save-time XSL transforms
slug: savetime_xsl_tr
date_published: 2002-12-09T22:30:15.000Z
date_updated: 2002-12-09T22:30:15.000Z
tags: tech
---

If you take a look at the developer documentation that’s just becoming available with the release of the first beta, you’ll see that [Office 11 supports XSL transforms](http://msdn.microsoft.com/library/default.asp?url=/library/en-us/dnofftalk/html/office12092002.asp) when saving a file as XML. It’s a great idea, basically allowing Office to natively export to *any* arbitrary output format on the fly.

So, let’s take it to the next step. A system-level registry of XSL transforms, perhaps cached locally with a definitive URL of their original locations, so you can see if there’s a new version when they’re called. Then expand the operating system’s save dialog to list these transformations as file type options whenever saving an XML file. This is something that could be implemented similarly on both Windows and OS X.

Then any application with an arbitrary data import format could supply its format as an XSL transformation, and apps could save to it through this registry. Maybe make the transformations discoverable through something analogous to WSDL, sorted by the MIME type of the content being saved.
