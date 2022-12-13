---
title: weblog api
slug: weblog_api
date_published: 2002-02-26T07:07:34.000Z
date_updated: 2002-02-26T07:07:34.000Z
---

Following up on the concept of [mindshare and market domination via APIs](http://www.dashes.com/anil/index.php?blogarch/2002_01_01_archive.php#9177215), I finally found a [common XML-RPC API for weblogs](http://techno-weenie.com/articles/rfc/weblog_api_1.shtml), which seems relatively well-designed. There’s also a [completely rearchitected API](http://techno-weenie.com/articles/rfc/weblog_api_2.shtml) that’s incompatible, which of course I like slightly better. Naturally the existing API doesn’t support versioning of the messages being received. I’m of the belief that the API in general would be improved by a tool-neutral name, a higher level of abstraction and extensibility, and a design more informed by some of the concepts (but not necessarily the weighty implementation) of [WebDAV](http://www.webdav.org/).

Show-stopper omissions in the API as proposed are a lack of time-based functions, including get/set post or comment time, and editing or deleting posts/comments by time or date range. This seems to be more fleshed out in the [Wasabii](http://wasabii.org/root/) spec. More discussion, as ever, in the relevant [Yahoo Group](http://groups.yahoo.com/group/weblog-devel).
