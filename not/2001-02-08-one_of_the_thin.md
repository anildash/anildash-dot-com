---
title: One of the things I
slug: one_of_the_thin
date_published: 2001-02-08T09:16:34.000Z
date_updated: 2001-02-08T09:16:34.000Z
---

One of the things I thought about a lot when Microsoft’s sites were down the other day was the reason that the flawed, single point of failure architecture was chosen.

The backstory was covered on Microsoft’s site years ago, when they moved to what they called a **Single IP solution**. This was back during the days of NT 4, and it was all rolled out about the time that Windows 98 was launched. You can read all about it at the ["Backstage" section on their site](http://www.microsoft.com/backstage/column_t2_1.htm).

But the server configuration created at that time, which remained in place until January 25th of this year, was based on a total control of the DNS servers remaining within Microsoft, at least until the new Single IP solution was stable. I suspect that the success of the technology (which was, dare I say it, *innovative* at the time) distracted the team from setting goals about outsourcing or colocating the DNS info once the project was complete.

It should have been obvious at the time, but perhaps someone kept putting off the outsourcing of DNS, for fear that a problem might develop in the Single IP solution which would require a return to the older system.

The irony in all of this, of course, was that the Single IP project greatly reduced the need for DNS servers in the first place, since only one IP address now needed to be mapped to the microsoft.com domain.
