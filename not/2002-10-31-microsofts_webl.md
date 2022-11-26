---
title: Microsoft's Weblog Software
slug: microsofts_webl
date_published: 2002-10-31T20:00:59.000Z
date_updated: 2002-10-31T20:00:59.000Z
tags: magazine, Technology and Entrepreneurship
---

Picture the following scenario: Microsoft has created a weblog tool that is designed to run inside the firewall at a company. It’s browser-accessible from any 4.0 or higher web browser and doesn’t require Windows on the client. It leverages their strengths by integrating with Office, and there’s no per-user client access fee. Then imagine if this weblogging tool were deployed to *millions* of users, all before anyone in the weblog community took notice.

That scenario is real.

### Background

Weblogs have been steadily gaining in attention and credibility in the 3 or 4 years since they first came to prominence. The power of a distributed, personally created medium with hundreds of thousands of authors spanning all social classes and geographic boundaries triggered excitement, hype, and cynicism that hadn’t been seen since the heights of the Internet boom.

[![Mock Microsoft Weblogger Box](/magazine/images/msblog.jpg)](http://www.wrongwaygoback.com/wetlogarchive/archive.asp?2002_02_17_archive.html#9865330)not the real thing

These accomplishments came largely on the back of three weblog tool platforms. Pyra’s Blogger and Userland’s Radio came first, followed more recently by Six Apart’s Movable Type. All three companies have an informal, first-person demeanor, with their founders, owners, and employees being weblog writers themselves. This is the case for most of the less-known weblogging platforms, as well. The casual nature of the tool creators’ efforts prompted occasional hand-wringing from time to time as various speculators would ask themselves, “When are the Big Guys going to try to muscle in on this realm?” That question, of course, spawned the [inevitable parody](http://www.wrongwaygoback.com/wetlogarchive/archive.asp?2002_02_17_archive.html#9865330).

While they were busy building audiences and focusing largely on the consumer market (with the exception of Userland, which has a significant commercial presence), Microsoft’s Office team developed a pair of products called [SharePoint](http://www.microsoft.com/sharepoint/).

### What is SharePoint?

In the recent Microsoft tradition of having two separate pieces of software that share the same name, there is a SharePoint Portal Server and SharePoint Team Services. [SharePoint Portal Server](http://www.microsoft.com/sharepoint/portalserver.asp) is another one of those overbuilt enterprise portal applications, a requisite for any large-scale development platform like .NET or Sun ONE or IBM’s WebSphere. Being a Microsoft application, it requires a Windows server, of course, and is as terminally boring as all of the products in its category, though it can be used to aggregate and present individual smaller websites within an organization, such as those created by SharePoint Team Services.

But [SharePoint Team Services](http://www.microsoft.com/frontpage/sharepoint/fastfacts.htm) (STS) is a workgroup-based or project-based intranet server, similar to what the original [Pyra](http://www.theobvious.com/archive/2000/05/01.html) application was trying to be. Perhaps the best illustration of this similarity is Microsoft’s inclusion of Team Services in the current version of [Project Server](http://www.microsoft.com/projectserver/). But even without the project management features, STS distinguishes itself with a focus on document management, contact management, and integration with Office stalwarts such as Outlook. The critical feature of STS, though, is a what’s referred to as "lists".

Lists, in a word, are weblogs.

### How It Works

Installing SharePoint is fairly easy. The millions of people running Office XP Professional with FrontPage, Office XP Developer, Project Server 2002, or the standalone FrontPage 2002 product already have it, either installed or ready to be installed with a few clicks. These applications shipped, complete with little blue gears logo for the product, in May of 2001. A standard installation Wizard enables it for those who, sensibly, didn’t install FrontPage by default when they set up Office.

[![SharePoint Entry Screen](/magazine/images/sharepointlist_thumb.png)](/magazine/images/sharepointlist.png)sharepoint entry screen

From a technical standpoint, SharePoint uses Microsoft SQL Server to provide data for the pages, all of which are dynamically generated. While the Portal Server uses the full-fledged version of SQL Server, Team Services can run on [MSDE](http://www.microsoft.com/sql/techinfo/development/2000/MSDE2000.asp), a desktop version of the same database engine. All of this back-end configuration can be done through a relatively friendly HTML interface built into the app, and individual pages can be customized with FrontPage. It’s probably possible to do this customization with a text editor and the raw HTML, but given the preponderance of proprietary ActiveX tags, few would be determined and masochistic enough to do so.

Things are considerably less ugly from a user standpoint. The pages of the interface are attractive and well designed, revealing a smooth workflow and task orientation that seems informed by actual user testing. You can add to a list (weblog) by simply typing into a regular HTML text area and clicking "save". Almost the entire functionality of the system is available through any 4.0 or higher browser, which seems to have been the intent of the development team. That some features are tied to Internet Explorer or the presence of Office on the client system seems like requirements foisted upon the product by some marketing or "Office Synergy Team" after the fact, but that’s purely speculative analysis based on the way tasks are integrated.

The strength of SharePoint, especially in comparison to its competitors in the realm of weblog software, is a keen sense of the importance of a user’s *other* information. Contact information and calendar appointments that can be imported with a click into Outlook, a consistent and well-designed searchable repository for Office documents such as Word files and Excel workbooks, and great support for threaded discussions all show directions that weblog software has yet to explore. It’s unlikely that any of the competitors in this realm will be taken seriously for some installs inside the firewall *until* those concerns, and issues like LDAP or NDS or Active Directory authentication, are addressed.

The strength of SharePoint is a sense of the importance of a user’s *other* information.

The other essential part of corporate integration that SharePoint nails is customization. There’s a [software development kit](http://msdn.microsoft.com/library/default.asp?url=/library/en-us/spsdk11/Intro/introduc.asp) documenting extensibility, complete with a proprietary markup language for modifying SharePoint sites, called [Collaborative Application Markup Language](http://msdn.microsoft.com/library/default.asp?url=/library/en-us/spsdk11/caml_schema/spxmlconcaml.asp) (CAML). The language even has its own active developer base, complete with [newsgroup](news://msnews.microsoft.com/microsoft.public.sharepoint.teamservices.caml). After deployment, system administrators have the all the resources of Microsoft’s [support infrastructure](http://www.microsoft.com/technet/treeview/default.asp?url=/technet/prodtechnol/sharepnt/default.asp). All of these resources haven’t gone unnoticed, either. The one player which seems to be fully aware of both the weblog space and SharePoint’s potential is [Ray Ozzie](http://www.ozzie.net/blog/)‘s Groove Networks, which has [fully embraced](http://www.groove.net/about/microsoft/sharepoint.html) the SharePoint platform while being completely aware of the attention and activity around weblogs. Aside from Groove, most weblog software companies are either unaware of or unwilling to acknowledge Microsoft’s participation in the realm, with the few [discussions of the tool](http://theflangynews.editthispage.com/2002/03/26) mentioning it only in passing, or in reference to Groove’s relationship.

### Resistance Ain’t Futile

So should everyone just pack it in and go home? Should today’s weblog software companies cede the enterprise and business markets to Microsoft’s endless cash and brutal marketing? Probably not. There are enough significant vulnerabilities in Microsoft’s strategy for SharePoint that their failure in this market seems *likely*, not just possible. First among these vulnerabilities is the fact that Microsoft is probably going to neuter the product.

![SharePoint's Logo](/magazine/images/gears.gif)sharepoint’s gear logo

They’ve already [announced](http://www.crn.com/Sections/BreakingNews/breakingnews.asp?ArticleID=36329) that SharePoint 2.0 will “integrate” Team Services and the Portal Server. Whether that means closer ties or the actual merging of the code base is still a subject for debate outside of Microsoft’s walls, but the threat such integration poses to a user interface that’s already derided *by a Microsoft employee* as "[too rigid and formal](http://sapid.com/tww/archives/2002/03/26.html)". Some of this clunkiness can be seen in the [Flash demo](http://www.microsoft.com/frontpage/sharepoint/howto.htm) of the application and in the [live mockups](http://www.sharepointsample.com/samplesites.htm) that show some sample installations. Despite the difficulties of use, it becomes clear that it’s easier to make a platform-neutral web product than to tie HTML to one operating system.

More to the point, Microsoft must be keenly aware that managing group projects through a browser-neutral interface when they’re still giving away browsers for free on Mac OS and Windows is *not* going to help the revenues of the Office team that developed SharePoint. Team Services marks the first time that any Office application could extend its functionality to other users in a workgroup without additional licensing fees, except in the limited sense of the document viewing applets that are downloadable for free.

What’s more, in an environment when real-world businesses are [finally getting the message](http://devedge.netscape.com/viewsource/2002/wired-interview/) about the value of standards-based web development, and are verging on using XHTML to deliver some of the long-promised benefits of the Semantic Web, SharePoint still relies on CAML, a proprietary scripting language, to generate HTML that’s clogged with proprietary and nonstandard markup that will only ever be viewable in a smaller and smaller share of the web audience. For a public site, there may be some tradeoffs that are made due to limited development resources, but even an all-Microsoft shop can hardly afford to use a team management tool whose output and discussions aren’t accessible in a PocketPC running a Microsoft OS.

Couple the technical weaknesses of SharePoint with its complete lack of support for the biggest areas of weblog development, such as RSS output, XML-RPC interfaces, and TrackBack support, and suddenly Microsoft’s presence in the realm doesn’t seem nearly as intimidating. Perhaps most damning, SharePoint requires not just a notoriously high-maintenance Windows server to run, but depends on the even less secure underpinnings of the FrontPage Server Extensions. With the increasing prevalence of wireless networks in the enterprise, system administrators are often unwilling to expose themselves to the risk of such frequently flawed platforms even *within* the firewall, especially when competing products run on free platforms.

### Conclusion

Microsoft has pieces in place that put it a full year ahead of any competitor

So how serious is the threat? To the overwhelming majority of personal weblog communities existing today, SharePoint is probably not going to have an impact in the short term. It’s possible that Microsoft will realize the potential of their bCentral service [hosting SharePoint sites](http://www.bcentral.com/products/sp/), and that the MSN team will seize the opportunity to improve the friendliness of the interface and turn it into a commercial mass-market product. The *likelihood* of that, however, is completely negligible. On the business side, though, Microsoft has pieces in place that put it a full year ahead of any competitor in the areas of network identity integration, document management, and project management functions. This advantage is probably negated by the significantly higher platform costs of a solution that requires a Windows server, even if there are no per-client costs.

The final analysis puts Microsoft on even footing with its much smaller competitors, which is both a tribute to their nimbleness and an indictment of their lack of focus on the business market. Given the resentment against Microsoft’s licensing changes, end-users’ familiarity with browser-based applications, and the newly resurgent eagerness of businesses to adopt centrally-managed knowledge management applications based on free or low-cost platforms, weblogs are ripe for a shot as the preferred Intranet knowledge management solution. Microsoft has entered this market, albeit with a slight stumble. Now that competitors are aware of their presence, it would behoove them to stake their claims in the market.
