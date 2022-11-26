---
title: I already knew Ray was
slug: i_already_knew
date_published: 2001-07-27T05:16:03.000Z
date_updated: 2001-07-27T05:16:03.000Z
---

I [already knew](http://www.dashes.com/anil/index.php?blogarch/2001_02_01_archive.php#2558697)[Ray](http://www.themaxx.com/bits/) was cool, but now he’s really gone above and beyond by helping me track down some bugs in my CSS code on Internet Explorer on the Mac. He sent me screenshots, code suggestions, and information, and it’s the kind of generosity that makes me so glad I run this site; I get to see just how wonderful people can be.

For the record, I had a  tag that was opened before the sidebar’s 
 but was closed *within* the 
 instead of *after* it. This caused the sidebar to stop rendering at that point, until I moved the 

 tag to after the 
.

Not that any of you really care that much about my page’s layout, but I wanted to mention what appears to be a browser anomaly for any of you who might be making CSS pages… Lesson learned: **It’s *still* a bad idea to improperly nest elements**.
