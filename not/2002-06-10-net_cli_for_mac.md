---
title: .NET CLI for Mac OS X
slug: net_cli_for_mac
date_published: 2002-06-10T19:35:02.000Z
date_updated: 2002-06-10T19:35:02.000Z
---

There’s some interesting findings if you read through the docs and source code for the [Common Language Infrastructure](http://msdn.microsoft.com/library/default.asp?url=/library/en-us/Dndotnet/html/mssharsourcecli.asp) component of Microsoft’s .NET framework. The entire infrastructure (which is what runs .NET code that’s been written) has been written for, and *already* compiles on, FreeBSD for x86. And all the hardware-specific parts are extracted into a Platform Abstraction Layer (the PAL is discussed in more detail [here](http://msdn.microsoft.com/msdnmag/issues/02/07/SharedSourceCLI/default.asp)) that should simplify any future ports.

What it means is, Mac developers should be able to [download](http://msdn.microsoft.com/downloads/sample.asp?url=/msdn-files/027/001/901/msdncompositedoc.xml&amp;frame=true) the framework and port it in relatively short order, given OS X’s BSD underpinnings. The only real work is translating x86 calls to PowerPC, but since the opposite’s been done fairly easily for the [Darwin x86](http://lists.apple.com/mailman/listinfo/darwin-x86) project, I am curious to see when it’ll happen.
