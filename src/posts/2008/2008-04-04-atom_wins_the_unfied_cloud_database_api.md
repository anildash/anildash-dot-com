---
title: "Atom Wins: The Unified Cloud Database API"
slug: atom_wins_the_unfied_cloud_database_api
date_published: 2008-04-04T21:04:06.000Z
date_updated: 2008-04-04T21:04:06.000Z
tags: [Best Of]
---

Almost five years ago, I got involved in a project that would eventually become [Atom](http://en.wikipedia.org/wiki/Atom_(standard)), a pair of matching standards functioning as a syndication format and a publishing protocol. Though its contentious genesis was in the world of blogging and feeds, what’s amazing is the improbable end result of the Atom community refining and debating the standard for half a decade.
**AtomPub has become the standard for accessing cloud-based data storage**. From Google’s [GData](http://code.google.com/apis/gdata/reference.html) implementation to Microsoft’s [unified storage platform](https://web.archive.org/web/20080517030059/http://dev.live.com/blogs/devlive/archive/2008/03/12/220.aspx) that includes SQL Server, Atom is now a consistent interface to build applications that can talk to remote databases, regardless of who provides them. And this milestone has come to pass with almost no notice from the press that covers web APIs and technology. A single common interface for keeping data in reliable cloud storage is as important a development as infrastructure-on-demand offerings like Amazon’s EC2 and S3 web services, and can radically impact the creation of applications for distributed social platforms like OpenSocial or the Facebook API.

Of course, there’s a lot more to the AtomPub story. There’s open source support from infrastructure-level implementations like [Apache Abdera](http://incubator.apache.org/abdera/) to application implementations as in [Movable Type](http://www.movabletype.org/) and interoperability testing as made possible by [The Ape](http://www.tbray.org/ape/). But those have been around for a while: Being able to build a program that doesn’t care if the backend is Google Base or SQL Server is new.

The reason this is a true milestone, and that it’s especially disappointing that the tech trade press hasn’t been paying attention, is because we’ve seem some remarkable announcements.

From Microsoft’s [David Treadwell](https://web.archive.org/web/20080511192047/http://dev.live.com/blogs/devlive/archive/2008/02/27/213.aspx):

> Microsoft is making a large investment in unifying our developer platform protocols for services on the open, standards-based Atom format (RFC 4287) and the Atom Publishing Protocol (RFC 5023). At MIX we are enabling several new Live services with AtomPub endpoints which enable any HTTP-aware application to easily consume Atom feeds of photos and for unstructured application storage (see below for more details). Or you can use any Atom-aware public tools or libraries, such as .NET WCF Syndication to read or write these cloud service-based feeds. …
> 
> The intent for these early, experimental releases are to gather valuable feedback from the community around our idiomatic and freely licensed extensions to AtomPub which deal with important service scenarios, such as URL formats, nested directories, image streams, and service metadata. You can read more about this on the Project Astoria team blog.

And from Google’s [Joe Gregorio](https://web.archive.org/web/20080405230542/http://googledataapis.blogspot.com/2008/04/google-data-apis-patent-license.html):

> We’ve always encouraged other developers to adopt Atom, the Atom Publishing Protocol, and the extensions that Google has created on top of those standards, but we realized the issue of patents may have held back some adopters. Well, those concerns end today as we are giving a no-charge, royalty-free license to any patents we have that you would need to implement Atom, AtomPub, or any of those extensions.

There’s clearly still work to be done, of course. I believe Microsoft will find Google’s licensing terms open enough for them to feel comfortable implementing GData-compatible APIs. Amazon should find a way to map these same APIs onto the [SimpleDB](https://aws.amazon.com/simpledb/) service, though I understand fundamental differences in architecture may make that a challenge. The multitude of smaller cloud-database vendors will find it easier to get adoption and customers if they can assert compatibility with these implementations.

But, put succinctly, **Google + Microsoft = AtomPub wins**. To paraphrase Dave Winer, the act of putting aside ego and saying a competitor’s API is good enough, and that you’re going to support it, is a brave and important act in the world of technology. That makes this convergence particularly exciting.

And it’s a real act of technological courage because *any* reasonably competent technology company can find reasons to object to any standard or API that’s ever presented. “We’d prefer it work *this* way.” “Your implementation is too verbose!” “What about just using this *other* technology?”

In the end, it doesn’t matter if a standard is perfect; All that matters is that it *works*. I am, by no means, the kind of person who thinks that anything adopted by two giant tech companies is always going to be acceptable, but the fact that there is also significant support for AtomPub from small, independent hackers is a pretty good sign that this victory is good for the web as a whole.

Now I just hope people make something really cool out of this. I want every program that thinks of itself today as a “blogging client” to reimagine their market as being a front-end to a database in the cloud. I want all the apps built on smart database abstractions to think about this new unified cloud API as an option they must support. And most of all, I want geeks to make something cool with this that we couldn’t do before.

Some key links:

- [IETF RFC 5023](http://tools.ietf.org/html/rfc5023), the Atom Publishing Protocol
- [A Unified Standards-Based Protocols and Tooling Platform for Storage from Microsoft](https://web.archive.org/web/20080517030059/http://dev.live.com/blogs/devlive/archive/2008/03/12/220.aspx), from George Moore, Microsoft’s GM for the Live platform
- [Google Data APIs protocol reference](http://code.google.com/apis/gdata/reference.html)
- [GData patent license](http://code.google.com/apis/gdata/patent-license.html)
