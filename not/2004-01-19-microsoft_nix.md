---
title: Microsoft *nix
slug: microsoft_nix
date_published: 2004-01-19T11:59:59.000Z
date_updated: 2004-01-19T11:59:59.000Z
tags: random ha-ha, tech
---

What if Microsoft shipped "Linux for Windows"?

On Friday, Microsoft released a [free download of Windows Services for Unix](http://www.microsoft.com/windows/sfu/downloads/default.asp) version 3.5, a significant upgrade to the Unix integration product they’ve been offering for about 5 years. I’ve used it before, mostly as an NFS client, but there’s some remarkable changes this time around.

The Services for Unix (SFU) are *free to download* and consist of an entire Unix environment installed as a native subsystem on Windows. For those of you who don’t know your Windows NT/2000/XP/2003 history, the NT kernel has always supported running multiple subsystems, and NT has always shipped with a Posix-compliant command-line subsystem, largely for checklist compatibility with some now-obsolete government requirements. Unlike tools like [Cygwin](http://www.cygwin.com/), which run on top of the standard Windows shell, SFU implements the Interix subsystem as a true peer to the Windows shell.

But to that base SFU 3.5 adds some extraordinary new features. Both the Korn and C shells are included. A single rooted file system is now supported, finally abandoning the need to include drive paths in applications or scripts. And speaking of scripts, SFU includes Perl 5.6.1. There’s even the full complement of standard Unix utilities, including awk, grep, sed, tr, cut, tar, cpio, less, at, cron and batch. Essential applications like bind, sendmail and ftp? Present. Even gcc, gdb, and make are in the package.

There’s a lot of other stuff, of course, including the first tools to expose Windows’ long-dormant file system support for [junctions](http://www.dashes.com/anil/2000/10/19/sysinternals_ha) as symbolic links in the Interix environment. There’s the above-mentioned NFS support. There’s all kinds of user account synchronization features. A real version of telnet.

But what’s most astounding, perhaps, is not the fact that I can now untar most perl scripts as-is and have them run on Windows. (I’ll be testing out Movable Type shortly, of course.) What amazes me is that this product has slipped under the radar for so long. Any bets as to whether Longhorn includes this functionality out of the box? And It seems to me that this collection of functionality will rapidly allow Windows users to cover 90% of the things that OS X users are doing with Darwin. Interesting.
