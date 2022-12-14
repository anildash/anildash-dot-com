---
title: I'm still obsessing over NTFS
slug: im_still_obsess
date_published: 2001-01-05T23:58:11.000Z
date_updated: 2001-01-05T23:58:11.000Z
---

I’m still obsessing over [NTFS mount points and junctions](http://www.dashes.com/anil/2000/10/19/sysinternals_ha) too. I’m working on something new, but until then, here’s **how to mount your CD-ROM onto an NTFS Junction Point**. First, make a folder somewhere on your Windows 2000 machine, let’s call it, oh, "cdrom". Then, go to a DOS prompt (yeah, yeah, I know *Command* prompt…) and change to the parent of that new directory and type:

mountvol cdrom \?\Volume{1c1caff2-e133-11d3-8316-806d6172696f}\

Of course, substitute your own folder name, blah blah blah. That’s the GUID for CD-ROM drives in there, it’s the same on all machines. I’m thinking something really cool could be done with this…
